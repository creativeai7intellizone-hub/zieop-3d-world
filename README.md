<div align="center">

# ZIEOP — World-Class Pro

### A cinematic, static-first creative-tech portfolio for **3D · Motion · Web · Experiments**

![Zieop World-Class Pro](zieop-readme-banner.jpg?v=1786810480)

</div>

---

## ✦ What is Zieop?

A premium, dark, cinematic portfolio for **3D objects, motion studies, interactive web experiments, and model showcases** — built entirely as static HTML with no framework, no backend, and no required database.

> Objects with presence.

The site delivers a single unified `index.html` (with a byte-identical `zieop.html` mirror) that hosts:

- **2** original local GLB models (Original Form I + II)
- **15** local GIF motion studies
- **9** numbered sections (01 → 09) covering Featured · Local Collection · 3D World · Model Vault · Art Wall · Motion · Lab · System · Contact
- **8** world media files — MP4 reels and JPG stills

![Zieop originals — local 3D collection](zieop-originals-preview.png?v=1786810480)

The screenshot above shows the **02 / LOCAL COLLECTION** section with Original Form I and Original Form II, each tagged `PBR · glTF 2.0 · Local · Web-ready` with a `Download GLB` action.

---

## 🎨 Design language

| Token | Value | Use |
|---|---|---|
| `--bg` | `#07090d` | Page background (deep cinematic dark) |
| `--panel` | `#0d1118` | Card surfaces |
| `--panel2` | `#111722` | Elevated surfaces |
| `--text` | `#f5f7fb` | Primary text |
| `--muted` | `#98a2b3` | Secondary text |
| `--accent` | `#7c5cff` | Primary violet accent |
| `--accent2` | `#12d7ff` | Secondary cyan accent |
| `--good` | `#57e389` | Success states |

**Font:** Inter / system stack — calm, editorial, screen-first.

**Visual direction:** Dark · Minimal · Cinematic · 3D-first · Editorial rather than crowded · Reduced-motion aware · Static-host friendly · Built around one final unified identity rather than versioned UI screens.

---

## 📦 Package inventory

| Asset | Count | Purpose |
|---|---:|---|
| Original local GLB models | 2 | Hero objects for Featured + Local Collection |
| Local model PNGs | 2 | Poster renders (Original Form I + II) |
| Local GIF motion archive | 15 | Loop studies / render previews |
| MP4 world reels | 4 | `media/world/*.mp4` — environment · creature · vehicle · hero |
| World JPG stills | 4 | `media/world/*.jpg` — creature · dragon · architecture · gallery |
| Live sections | 9 | Numbered `01 → 09` navigation |
| README banner | 1 | `zieop-readme-banner.jpg` |
| Gallery contact sheet | 1 | `zieop-readme-gallery.jpg` |
| Site preview | 1 | `zieop-originals-preview.png` |

---

## 🧭 Section map (01 → 09)

| # | Section | Anchor |
|---:|---|---|
| 01 | Selected Works | `#featured` |
| 02 | Local Collection | `#collection` |
| 03 | 3D World | `#world` |
| 04 | Model Vault | `#open` |
| 05 | Art Wall | `#art` |
| 06 | Motion Archive | `#motion` |
| 07 | Zieop Lab | `#lab` |
| 08 | System | `#system` |
| 09 | Contact | `#contact` |

**Stats strip:** 02 ORIGINAL 3D ASSETS · 04 OPEN MODEL PICKS · 15 MOTION STUDIES · 09 CORE SECTIONS.

---

## 🗃 Model Vault

The UI serves the two bundled Zieop models locally. Each card has a direct `Download GLB` action pointing to the raw GitHub URL.

| File | Size | Use |
|---|---:|---|
| `zieop-model-01.glb` | 28 MB | Original Form I — hero creature |
| `zieop-model-02.glb` | 30 MB | Original Form II — companion piece |
| `zieop-model-01.png` | 270 KB | Poster render for Form I |
| `zieop-model-02.png` | 385 KB | Poster render for Form II |

The mirror copy under `model-vault/` is kept for archival / redistribution convenience. See [`MODEL-VAULT.md`](./MODEL-VAULT.md) for the local-first policy.

### Open model picks

The active page surfaces four open-source showcase models alongside the originals — referenced for study purposes only with their upstream sources credited. Each card links to the upstream model page and respects its license terms.

---

## 🎬 Motion Archive (15 studies)

| Range | Theme |
|---|---|
| `zieop-preview-01.gif` → `05` | Loop studies |
| `zieop-preview-06.gif` → `10` | Character motion |
| `zieop-preview-11.gif` → `15` | Compositing + VFX |

The page loads them lazily as the visitor scrolls and offers a searchable filter (`/` focuses the search field, dropdown filter for `01–05 / 06–10 / 11–15`).

---

## 🌐 3D World media

| File | Type | Use |
|---|---|---|
| `media/world/zieop-world-03.mp4` | video | Hero world reel |
| `media/world/zieop-world-06.mp4` | video | Environment study |
| `media/world/zieop-world-07.mp4` | video | Character study |
| `media/world/zieop-world-08.mp4` | video | Vehicle study |
| `media/world/zieop-world-10.jpg` | image | Mechanical creature still |
| `media/world/zieop-world-14.jpg` | image | Dragon sculpture still |
| `media/world/zieop-world-15.jpg` | image | Architecture still |
| `media/world/zieop-world-gallery.jpg` | image | World archive collage |

All World media is bundled under `media/world/` and is served by Zieop itself. No external media-host links are required.

---

## ⚙ Runtime dependencies

- **3D viewer** — Google-hosted `model-viewer` v4.0.0 (loaded from `ajax.googleapis.com`)

The interactive open-model showcase loads four showcase GLBs from their upstream sources. The supplied Zieop GLB, PNG, GIF, MP4 and README images remain local to this package.

---

## 🚀 Hosting

### Vercel (current production)

1. Deploy the `zieop` folder
2. Keep `index.html` at the deployment root
3. No build command is required
4. No framework adapter is required

Live at **[zieop.vercel.app](https://zieop.vercel.app)**.

### Other static hosts

Any normal static host that can serve HTML, CSS, JavaScript, PNG/JPG/GIF, MP4 and GLB files can serve the package.

---

## 🎹 Interaction map

- `Featured` → selected work presentation
- `3D World` → atmospheric visual world
- `Open Models` → open-source 3D gallery
- `Art Wall` → visual preview wall
- `Motion` → searchable 15-item motion archive
- `Lab` → experimental direction
- `Contact` → collaboration CTA
- `/` → focuses the motion search field
- Local model fullscreen controls → available on original model cards
- Motion and Art Wall cards → open in the visual preview modal

---

## ✅ Final QA checklist

- [x] `index.html` exists
- [x] `zieop.html` matches `index.html` byte-for-byte
- [x] 2 local GLBs present
- [x] 2 local model PNGs present
- [x] 15 motion GIFs present
- [x] Motion script generates the exact `01`–`15` filenames
- [x] Main section anchors exist (01 → 09)
- [x] Navigation links resolve to existing sections
- [x] Skip link resolves to `#content`
- [x] Local fullscreen controls have accessible labels
- [x] Modal has dialog semantics
- [x] `.gitignore` is ready to use
- [x] README visual assets are packaged
- [x] No active `v1`–`v7` UI naming is used
- [x] Third-party licenses are kept separate from project-code licensing

---

## 📁 Folder map

```text
zieop/
├── index.html                  # Primary static-hosting entry point
├── zieop.html                  # Matching standalone mirror
├── .gitignore                  # Repo-ready ignore rules
├── zieop-gitignore             # Compatibility copy of ignore rules
├── zieop-model-01.glb          # Original 3D asset 01 (28 MB)
├── zieop-model-01.png          # Poster render for Form I
├── zieop-model-02.glb          # Original 3D asset 02 (30 MB)
├── zieop-model-02.png          # Poster render for Form II
├── zieop-preview-01.gif … 15   # 15-piece motion archive
├── zieop-readme-banner.jpg     # README hero banner
├── zieop-readme-gallery.jpg    # README contact sheet
├── zieop-originals-preview.png # Site preview (Local Collection)
├── zieop-readme.md             # Full project documentation
├── zieop-license.txt           # Code/license + third-party asset notice
├── MODEL-VAULT.md              # Model Vault policy
├── REPO-MIGRATION.md           # GitHub/Vercel cutover checklist
├── model-vault/                # Mirror copy of GLB assets
│   ├── index.md
│   ├── zieop-model-01.glb
│   └── zieop-model-02.glb
└── media/world/                # World reels + stills
    ├── zieop-world-03.mp4
    ├── zieop-world-03.jpg
    ├── zieop-world-06.mp4
    ├── zieop-world-06.jpg
    ├── zieop-world-07.mp4
    ├── zieop-world-07.jpg
    ├── zieop-world-08.mp4
    ├── zieop-world-08.jpg
    ├── zieop-world-10.jpg
    ├── zieop-world-14.jpg
    ├── zieop-world-15.jpg
    └── zieop-world-gallery.jpg
```

---

## 🛡 Asset / license notes

The supplied local files (`zieop-model-*`, `zieop-preview-*`, `zieop-world-*`, renders, posters) are treated as source-project assets. This package does **not** assume ownership or automatically relicense those files.

The project/code license is documented separately in [`zieop-license.txt`](./zieop-license.txt). The four open-source showcase models loaded from upstream sources retain their individual licenses.

### Contact placeholder

The page currently uses `hello@zieop.com` as the contact CTA address. Replace that address with the real portfolio email before publishing if `hello@zieop.com` is not your intended inbox.

---

## 📜 License

© Zieop. Bundled model assets retain their individual licenses (see `models/<name>/LICENSE.md`). Open-source showcase models retain their individual upstream licenses.
