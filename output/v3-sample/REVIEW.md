# Flame v3 sample review

The 17-pose sample is complete: six idle frames, five paw-greeting frames, and six poses crossing the downward head-turn boundary. It is a comparison prototype, not an installable pet release. It does not declare a new sprite format or modify the installed v2 pet.

## Assessment

- **Head turn: the strongest improvement.** The seated body stays much steadier. The largest neighboring silhouette-area ratio drops from 1.222 in the v2 excerpt to 1.024 in the v3 sample (22.2% versus 2.4%). The 157.5° → 180° boundary drops from 1.222 to 1.006. This is a measurement of occupied pixels, not a perceptual-quality score. The final two downward-left poses remain subtle, so a complete direction set would need further semantic review.
- **Idle: modest improvement.** The complete blink remains readable and the body is well registered. The maximum adjacent area ratio is 1.011 versus 1.027 for v2. The artistic difference at pet size is small.
- **Paw greeting: an alternative expression.** The sample completes a lift-and-return, with stable registration and a friendly peak pose. Its intervening poses feel more neutral than v2; the original greeting remains a reasonable choice.

Recommendation: continue v3 development around the head-turn consistency, preserve Flame's sculpted-clay identity, and choose the greeting on visual preference. A complete release would need coherent eight-pose direction rows, full-atlas validation, and independent direction reviews. This six-pose study is not a replacement atlas row.

## Review controls

Open `preview.html` locally. The images are embedded, so playback does not require a server or network connection. Select a study, pause, step frames, reduce playback speed, or switch among warm, dark, white, and checker backgrounds. V2 and V3 use the same timing. The head turn runs forward and backward with no generated intermediate frames.

Each sprite cell is 192 × 208 pixels. On narrow phone layouts, the viewer reduces display size to fit; desktop shows native size. PNG frames and looping lossless WebP files are included separately.

## Verification

- All 17 candidate frames are nonempty and clear the 2-pixel outer-edge check.
- Every source contains the requested number of complete, separated pose groups.
- Frame extraction uses Hatch Pet component recovery, one shared scale per strip, and lower-body registration against v2's neutral cell. No artwork or in-between poses are synthesized by code.
- A single Hatch Pet edge cleanup preserves alpha exactly.
- All 42 exported playback frames across the six V2/V3 WebP files decode with identical alpha and identical white/dark RGB composites to their source PNGs.
- Independent visual review passes all three studies, with the expression and directional caveats above. The reviewer inspected static sequences; its animation viewer did not play WebP. The parent checked the browser viewer and frame controls separately.
- An initially reported gray triangle was rechecked on exact PNGs and the dark browser background: it is attached rear-ear fur, not a detached object. No repair was needed.
- One idle generation was rejected for touching the outer canvas edge; the accepted regeneration uses wider cyan margins.

## Provenance

Generated using built-in ImageGen with Flame's existing reference images. The exact underlying model is not exposed, and v2's original records do not identify its model either. No claim of a verified model upgrade is made. Prompts, including the idle repair instruction, are in `generation-prompts.md`.
