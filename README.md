# Flame 🐾

A sable-and-white Sheltie companion for Codex and ChatGPT, with sculpted clay fur, a friendly paw wave, and thirteen expressions—including a howl.

<p>
  <img src="output/emotes/waving.webp" width="192" height="208" alt="Flame waving hello">
  <img src="output/emotes/idle.webp" width="192" height="208" alt="Flame resting calmly">
  <img src="output/emotes/howling.webp" width="192" height="208" alt="Flame howling">
</p>

## Download

- **[Pet package](https://github.com/banterle-hash/flameatar/releases/latest/download/flame-pet-share.zip)** — the desktop pet and installation instructions, about 1.7 MB.
- **[Full avatar and emote pack](https://github.com/banterle-hash/flameatar/releases/latest/download/flame-avatar-pack.zip)** — the pet, transparent avatar, all expressions, and an interactive gallery.
- **[Sprite sheet](output/flame/spritesheet.webp)** — for supported custom-pet uploaders.

## Install on desktop

1. Download and extract the pet package.
2. Place the entire `flame` folder in `~/.codex/pets/` (or the `pets` directory under your custom `CODEX_HOME`). Back up any existing Flame folder first.
3. Confirm these two files exist:

   ```text
   ~/.codex/pets/flame/pet.json
   ~/.codex/pets/flame/spritesheet.webp
   ```

4. Open **Settings → Pets → Refresh**, then choose **Flame**.
5. Enter `/pet` to wake him.

For ChatGPT web accounts with Pets enabled, use **Settings → Personalization → Pet → Upload pet** and select the extracted `spritesheet.webp` image, not the ZIP. Desktop pets do not automatically sync to the web. See the [official Pets documentation](https://learn.chatgpt.com/docs/pets).

## Expressions

| Expression | Behavior |
| --- | --- |
| Hello there | Friendly paw greeting; also used for hover |
| Just here | Calm resting and blinking |
| On the move → / ← | Rightward and leftward trots |
| Your turn | Expectant tilt and asking paw |
| Thinking it through | Concentrating on work |
| All ready | Satisfied and attentive |
| Oh no | Lowered head and disappointed ears |
| Little celebration | A playful hop, available as a separate emote |
| Sleepy | A resting expression |
| With love | Hugging a heart |
| Oh! | Surprise |
| Awooo! | An animated howl |

The pack has thirteen PNG expressions, ten looping animated WebP emotes, and three static WebP emotes. The pet rests calmly and greets you on hover. Celebration and howling remain standalone emotes.

## Preview and files

Extract the full pack and open `preview.html` in a browser. It includes light/dark backgrounds, pause/play controls, and individual downloads. From a repository checkout, open `output/preview.html`.

- `output/avatar.png` and `output/avatar.webp`: transparent 1024 × 1024 avatar.
- `output/flame/`: installable manifest and transparent sprite sheets.
- `output/emotes/`: finished reaction images and animations.
- `output/emotes.json`: filenames and animation timings.
- `output/animation-contact-sheet.png`: all native sprite frames.
- `output/SHARE.md`: portable installation and sharing instructions.

This pack retains the v1 format: an 8 × 9 atlas, 192 × 208 pixel cells, and a total size of 1536 × 1872. The host's five-frame `jumping` slot is deliberately a paw greeting for hover; the original celebratory hop is still `output/emotes/jumping.webp`. Directional-look rows from the v2 format are not included.

Artwork was created with OpenAI image generation and processed with Hatch Pet tools. Transparent fur edges were cleaned while preserving alpha, and WebP assets use lossless compression. Frame counts, timing, transparency, atlas layout, and package integrity were validated; the preview was visually checked on light and dark backgrounds.

Only finished artwork and sharing documentation are published here. Reference photos, videos, local paths, and working generation files are excluded. Flame is a custom pet project, not an official OpenAI mascot.
