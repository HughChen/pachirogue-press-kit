# PachiRogue Press Kit

Public press kit for **PachiRogue**, hosted on GitHub Pages.

**Live site:** https://hughchen.github.io/pachirogue-press-kit/

## What’s included

| Path | Purpose |
|------|---------|
| `index.html` / `styles.css` | On-page press kit (factsheet, pitch, features, media, download) |
| `Factsheet.txt` | Plain-text factsheet |
| `PressKit_PachiRogue/` | Downloadable asset pack (organized folders) |
| `PressKit_PachiRogue.zip` | Same pack, one-click download from the page |
| `assets/images/` | Lightweight copies used by the webpage |

### Asset pack layout

```
PressKit_PachiRogue/
├── 01_Logos_and_Icons/
├── 02_Screenshots/          ← add gameplay shots here
├── 03_Key_Art_and_Banners/
├── 04_GIFs_and_Short_Clips/ ← add GIFs / short clips here
└── Factsheet.txt
```

## Fill in before sharing widely

Edit `index.html`, `Factsheet.txt`, and `PressKit_PachiRogue/Factsheet.txt`:

- [ ] Press email / contact
- [ ] Location
- [ ] Price (or confirm TBD)
- [ ] Social links
- [ ] YouTube trailer embed + download link
- [ ] Gameplay screenshots (`02_Screenshots/`)
- [ ] Core-loop GIF (`04_GIFs_and_Short_Clips/`)
- [ ] Optional: Google Drive mirror URL for the zip

After adding assets, regenerate the zip:

```bash
rm -f PressKit_PachiRogue.zip
zip -r PressKit_PachiRogue.zip PressKit_PachiRogue -x "*.DS_Store"
```

## GitHub Pages

1. Repo **Settings → Pages**
2. Source: **Deploy from a branch**
3. Branch: `main` / `/ (root)`
4. Save — site publishes at `https://hughchen.github.io/pachirogue-press-kit/`

## Local preview

```bash
cd pachirogue-press-kit
python3 -m http.server 8080
# open http://localhost:8080
```
