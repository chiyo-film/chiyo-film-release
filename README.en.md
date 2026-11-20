# Chiyo Film

English · **[한국어](README.md)**

**Free · Cull, develop RAW, add the film look and export in one app · Also inside Lightroom Classic & Photoshop · 154 film looks**

A film-emulation editor for Mac. Film looks built from real datasheet curves, plus photo adjustments, face retouching, frames and cinema looks. From 1.7 it also works on its own as a **photo library**: open a folder, cull, develop RAW, finish like film and export.

![Before/after: N102 Warm snapshot · S102 Classic slide · C601 Cool night · N101 Natural portrait · N104 Soft portrait · M301 Classic B&W](img/00-before-after.jpg)

<sub>Left: original · Right: Chiyo Film (film + exposure, white balance, grain, halation). Example photos are CC0 (public domain) from Wikimedia Commons.</sub>

![Chiyo Film library](img/13-library-en.jpg)

![Chiyo Film editor in English](img/12-english-ui.png)

## Download

**[Get the latest release](../../releases/latest)** → `ChiyoFilm-1.8.0.pkg`

- macOS 13 or later, Apple Silicon (M1 or later)
- Lightroom Classic and/or Photoshop 2025 or later (optional — the library and editor work on their own)
- RAW: cameras macOS supports, plus Sony A7 V · A7R VI Compressed RAW 2 (developed with the bundled LibRaw; no Adobe DNG Converter needed)
- Manual: **[ChiyoFilm-Manual-EN.pdf](ChiyoFilm-Manual-EN.pdf)**
- Licence: **[LICENSE.en](LICENSE.en)** (English translation; the Korean [LICENSE](LICENSE) governs) — free test version for personal, non-commercial use; no redistribution; your output photos are yours to use freely.

The app follows your Mac's language. To switch: **Advanced › 언어 · Language** (Auto · 한국어 · English).

## Install

1. Quit Photoshop and Lightroom Classic (save your work first).
2. Open `ChiyoFilm-1.8.0.pkg`. If macOS says "unidentified developer", **right-click › Open** in Finder, or **System Settings › Privacy & Security › Open Anyway**.
3. The editor app, the Photoshop plugin and the Lightroom plugin are installed together.
4. **Once in Lightroom:** Settings › External Editing › Additional External Editor › Choose › `/Applications/Chiyo Film.app`
   - File format **TIFF or PSD**, **16-bit**, colour space as you usually work (ProPhoto RGB or Adobe RGB)
   - Preset › Save Current Settings as New Preset › "Chiyo Film"

## Use

| Where | How |
|---|---|
| Lightroom Classic | Right-click a photo › Edit In › **Chiyo Film** (⌥⌘E) → edit → **Apply** (Return) → appears next to the original |
| Lightroom, many photos | File › Plug-in Extras › **Chiyo Film: Apply to Selected Photos…** (TIFF / JPEG / PSD, added to the catalogue) |
| Photoshop | Plugins › Chiyo Film › **Open Chiyo Film Editor** → Apply adds a new layer |
| **Photo library (new)** | Open `Chiyo Film.app` › Open Folder (⌘O) → rate and flag in Grid / Loupe (1–5 · P · X) → Enter to edit → ⌘E to export |
| Standalone | Drop JPEG · TIFF · PSD · RAW files on `Chiyo Film.app` |
| Batch in the editor | File › **Apply to Multiple Photos…** (⇧⌘B) |
| 2–4 photos on one canvas | File › **Create Multi-Photo Layout…** (⇧⌘L) |

> **Tip:** open RAW files in the library and start with **RAW Development** (exposure, white balance, highlight recovery). If you use Lightroom, developing there first and sending the photo to Chiyo Film still works as before.

## Highlights (1.8)

- **Match Set (new):** evens out brightness, white balance, skin colour (measured per face), contrast and saturation of a set against a reference photo, with per-photo changes, before/after previews, a strength slider and one-step ⌘Z.
- **RAW for every camera brand (new):** the ‘Like the camera JPEG’ profile learns each camera model's own brightness and colour (skin included) from the JPEG inside its RAWs — within ±0.07 EV and 0–4° of skin hue on Canon, Nikon, Fujifilm, Panasonic, OM System, Pentax and Sony samples. Auto chromatic aberration measured on the photo (no lens data needed); Fujifilm X-Trans in the built-in converter.
- **Photo library (new):** open a folder for Grid · Loupe · Compare · Auto Cull. Rate, flag and colour-label from the keyboard (1–5 · P · H · X · 6–9), filters and smart collections (edited, 4 stars & up, possibly blurry, eyes closed, bursts). Edits save next to each photo in a `.chiyo` file (no catalogue); RAW ratings and labels also go to `.xmp` for Lightroom and Bridge.
- **Auto-cull help (new):** burst grouping with a suggested best shot; blur, missed focus, closed eyes and exposure flags.
- **RAW Development (new):** exposure, white balance, highlight recovery and shadows with macOS's RAW engine, keeping up to 2 stops above white. Sony A7 V · A7R VI open too. RAW+JPG as two photos or one.
- **Many photos at once (new):** ⌘/⇧-click multi-select, **Sync** (choose parts) and **Auto sync**, copy / paste edits, apply the previous edit, **virtual copies** (⌘'), right-click menus.
- **Export (new):** presets for web / social, print TIFF, Instagram 4:5, original size and Photoshop PSD; JPEG · HEIC · TIFF · PSD with size estimate, naming templates and a background queue. Right from the editor and loupe (⌘E), or just the picks.
- **1.8.0:** place the light leak with handles on the photo (like a linear gradient mask), and more natural dust and fibres.
- **Basic adjustments like Lightroom:** Highlights and Whites recover highlights naturally and sliders respond instantly; auto skin tone stays on the face.
- **Spectral film colour:** models each film layer's spectral sensitivity and, for print stocks (cinema print 2383, paper), the dyes printing onto each other. Reds and skin come out cleaner and less muddy; cinema print skies turn teal on their own. New edits use it by default; edits saved earlier open unchanged (Adjust › Film › Color science).
- **English interface**
- **Picks for this photo:** suggests 3–5 looks for each photo from its colours, subject and mood, with a reason.
- **30 cinema looks:** moods inspired by Japanese, Korean and world cinema (e.g. "Seaside Sisters in Summer — Kore-eda Hirokazu · Our Little Sister feel"), tuned by measuring stills and reading cinematography notes. Interpretations only — not affiliated with any filmmaker or studio, and no film stills ship with the app.
- **Film frames:** 2.39 scope and 1.85 flat letterbox, subtitle scene.
- **Develop & print:** push/pull development, printer points R·G·B, preflash, print toe/shoulder shape, bleach bypass (creative model).
- **Texture & optics:** grain and halation scaled to film format (half frame → 4×5), datasheet-based grain, diffusion filters (Black mist, White mist, Glimmer, Cine bloom — maskable), lens chromatic aberration and coma.
- **154 film looks:** 59 rendered from characteristic curves digitised from manufacturers' datasheets. Own short codes (e.g. N101 · Natural portrait) with a small "~ feel" line naming the stock it references.
- **Photo adjustments like Lightroom:** Basic, Tone Curve (incl. Luminance), Color Mixer, Color Grading, Precision Color (lift/gamma/gain/offset, hue curves), Detail, Lens Corrections.
- **Face retouch & skin tone:** blemish removal (moles kept unless you choose), dark circles, even skin with texture kept, contouring; skin-tone uniformity with a colour wheel.
- **Masks:** radial, linear, brush, luminance, colour range, auto subject / person / sky.
- **Frames & layouts:** 26 frames (palette, captions, film strip, contact sheet, deckle, textures), 2–4 photo layouts with carousel export.
- Reference-photo look matching, `.cube` LUT export, GPU real-time preview, histogram / waveform / RGB parade.
- Everything runs locally on your Mac — no account, no internet.

![Cinema looks](img/09-cinema-looks.jpg)

<sub>Cinema look examples on CC0 photos (not film stills). Left original · right look.</sub>

![Film frames](img/10-cinema-frames.jpg)

![Loupe](img/14-loupe.jpg)

![Syncing several photos](img/15-editor-sync.jpg)

## Changes

See [Releases](../../releases).

## Reporting problems

Create a report with **Advanced › Create Problem Report File…** and attach it to an [Issue](../../issues) with your macOS / Photoshop / Lightroom versions and the photo format. Please don't upload personal photos.

## Uninstall

```sh
sudo "/Library/Application Support/Chiyo Film/1.8.0/uninstall.sh"
```

Your presets and favourites (`~/Library/Application Support/Chiyo Film`) are kept.

---

Free test version, provided without any warranty (see the [licence](LICENSE.en)). Keep your originals backed up. Film looks are expressive models based on public characteristic curves, datasheets and scans; they are not guaranteed to match real film. Film and manufacturer names are trademarks of their respective owners and are used only to describe which stock a look references; Chiyo Film is not affiliated with them. Example photos are CC0.
