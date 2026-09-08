# Codex Avatars

Custom avatars, animated pets, and emote packs for Codex and compatible ChatGPT surfaces.

## Meet Flame 🐾

A sable-and-white Sheltie companion for Codex and ChatGPT, with sculpted clay fur, a friendly paw wave, and thirteen expressions—including a howl. The desktop pet also has sixteen looking directions.

<p>
  <img src="output/emotes/waving.webp" width="192" height="208" alt="Flame waving hello">
  <img src="output/emotes/idle.webp" width="192" height="208" alt="Flame resting calmly">
  <img src="output/emotes/howling.webp" width="192" height="208" alt="Flame howling">
</p>

## Download

### [Download Flame](https://github.com/banterle-hash/codex-avatars/releases/latest/download/flame-v2.zip)

The desktop pet, ready to install—with a paw greeting and sixteen looking directions.

Other downloads:

- [ChatGPT web version](https://github.com/banterle-hash/codex-avatars/releases/latest/download/flame-pet-share.zip) — contains the smaller sprite sheet required for web upload.
- [Avatar & emote pack](https://github.com/banterle-hash/codex-avatars/releases/latest/download/flame-avatar-pack.zip) — optional artwork, reactions, and an interactive gallery. Includes the web-compatible pet; use **Download Flame** above for the desktop pet with directional looks.

## Install on desktop

1. Select **Download Flame** above and extract the ZIP.
2. Place the entire `flame` folder in `~/.codex/pets/` (or the `pets` directory under your custom `CODEX_HOME`). Back up any existing Flame folder first.
3. Confirm these two files exist:

   ```text
   ~/.codex/pets/flame/pet.json
   ~/.codex/pets/flame/spritesheet.webp
   ```

4. Open **Settings → Pets → Refresh**, then choose **Flame**.
5. Enter `/pet` to wake him.

## Use on ChatGPT web

Download and extract the **ChatGPT web version** above. For accounts with Pets enabled, use **Settings → Personalization → Pet → Upload pet** and select `flame/spritesheet.webp` from that package. Upload the image, not the ZIP. Desktop pets do not automatically sync to the web. See the [official Pets documentation](https://learn.chatgpt.com/docs/pets).

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
- `output/flame-v2/`: v2 desktop manifest and sprite sheet; install these together in a folder named `flame`.
- `output/flame/`: classic v1 manifest and transparent sprite sheets, including the web-compatible sheet.
- `output/emotes/`: finished reaction images and animations.
- `output/emotes.json`: filenames and animation timings.
- `output/animation-contact-sheet.png`: all native sprite frames.
- `output/SHARE.md`: portable installation and sharing instructions.

## Sprite formats

**Download Flame** uses sprite format v2 for compatible desktop hosts. The **ChatGPT web version** uses v1 because the web uploader requires a transparent 1536 × 1872 image. Use the web package on older desktop hosts that require v1, too.

| Version | Atlas | Dimensions | Looking directions |
| --- | --- | --- | --- |
| Desktop v2 | 8 × 11 | 1536 × 2288 | 16 |
| Classic v1 / web | 8 × 9 | 1536 × 1872 | None |

Both formats use 192 × 208 pixel cells. V2 preserves the original nine animation rows and declares `spriteVersionNumber: 2`. The host's five-frame `jumping` slot is deliberately a paw greeting for hover; the original celebratory hop is still `output/emotes/jumping.webp`.

## Credits

Artwork was created with OpenAI image generation and processed with Hatch Pet tools. Transparent fur edges were cleaned while preserving alpha, and WebP assets use lossless compression. Frame counts, timing, transparency, atlas layout, and package integrity were validated; the preview was visually checked on light and dark backgrounds.

Only finished artwork and sharing documentation are published here. Reference photos, videos, and working generation files are excluded. Flame is an independent custom pet project.
