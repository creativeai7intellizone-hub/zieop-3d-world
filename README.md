# Zieop — World-Class Pro

Premium creative-tech portfolio for 3D, motion, interactive experiments, and a self-hosted model vault.

## Included

- Interactive local GLB viewing
- Local model downloads
- Motion archive with search/filter
- 3D World, Art Wall, Lab, System, and Contact sections
- Functional Start a Conversation modal
- GitHub Source Code button targeting `creativeai7intellizone-hub/zieop`
- Static-hosting friendly entrypoint (`index.html`)

---

## 🗃 Model Vault

Zieop ships a **self-hosted 3D model vault** — every model displayed in the site UI is bundled inside this repository so visitors can download from Zieop itself rather than an upstream host.

### Current local models

| File | Size | Purpose |
|---|---|---|
| `zieop-model-01.glb` | 28 MB | Hero creature / character |
| `zieop-model-02.glb` | 30 MB | Secondary showcase model |
| `zieop-model-01.png` | poster | Hero preview |
| `zieop-model-02.png` | poster | Secondary preview |

All `.glb` files live at the **repository root** so the relative `src="..."` paths inside `index.html` resolve correctly when served as static files. The mirrored copy under `model-vault/` is kept for archival / redistribution convenience.

### 📥 Download

Visitors get a "Download" button on every model card. Each button resolves to the raw GitHub URL:

```
https://raw.githubusercontent.com/creativeai7intellizone-hub/zieop-3d-world/main/zieop-model-XX.glb
```

This keeps downloads under the Zieop GitHub organisation — no third-party host, no broken CDN links.

### 🔒 License & attribution policy

The Khronos `glTF Sample Assets` catalog contains models with **different license and attribution requirements**. Zieop does **not** bulk-copy from upstream.

For any model redistributed under `model-vault/`, the canonical layout is:

```text
models/
  <model-name>/
    <model-name>.glb
    LICENSE.md
    ATTRIBUTION.md
```

If you add a new model:
1. Drop the `.glb` + its `LICENSE.md` + `ATTRIBUTION.md` under `models/<name>/`.
2. Reference it from `index.html` with a stable relative path.
3. The Download button points to `models/<name>/<name>.glb` in this repo.

**Do not** mark upstream catalogs wholesale as CC0 — each model carries its own terms.

---

## Deploy

The site is static and suitable for Vercel. Upload the repository root and use `index.html` as the entrypoint.

Recommended `vercel.json`:

```json
{
  "version": 2,
  "builds": [{ "src": "*.html", "use": "@vercel/static" }],
  "routes": [{ "src": "/(.*)", "dest": "/$1" }]
}
```

Deploy command (Vercel CLI):

```bash
npx vercel deploy --prod --yes --token "$VERCEL_TOKEN"
```

---

## 3D World media update

The final build replaces the abstract orbit-only World section with a curated visual-world experience. It includes local MP4 reels and JPG stills generated from the supplied Zieop motion archive. All World media is bundled under `media/world/` and is served by Zieop itself.

### World media

- `media/world/zieop-world-03.mp4` — hero world reel
- `media/world/zieop-world-06.mp4` — environment study
- `media/world/zieop-world-07.mp4` — character study
- `media/world/zieop-world-08.mp4` — vehicle study
- `media/world/zieop-world-10.jpg` — mechanical creature still
- `media/world/zieop-world-14.jpg` — dragon sculpture still
- `media/world/zieop-world-15.jpg` — architecture still
- `media/world/zieop-world-gallery.jpg` — world archive collage

No external media-host links are required for this section.

---

## Motion archive

15 curated previews — `zieop-preview-01.gif` through `zieop-preview-15.gif` — sit at the repository root. The site loads them lazily as the visitor scrolls.

| Range | Theme |
|---|---|
| 01–05 | Loop studies |
| 06–10 | Character motion |
| 11–15 | Compositing + VFX |

---

## License

© Zieop. Bundled model assets retain their individual licenses (see `models/<name>/LICENSE.md`).
