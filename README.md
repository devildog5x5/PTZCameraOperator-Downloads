# PTZ Camera Operator — Downloads

This repository hosts **release binaries** and a **download page** for [PTZ Camera Operator](https://github.com/devildog5x5/PTZ_Interface).

- **Download page (external URL):** [https://devildog5x5.github.io/PTZCameraOperator-Downloads/](https://devildog5x5.github.io/PTZCameraOperator-Downloads/) — after enabling GitHub Pages (see below).
- **Latest build:** [releases/latest/](releases/latest/) — installer, portable ZIP, and executable.

## Contents

| File | Description |
|------|-------------|
| **PTZCameraOperatorSetup-1.0.0.exe** | Windows installer (recommended) |
| **PTZCameraOperator-Portable-v1.0.0.zip** | Portable build — extract and run `PTZCameraOperator.exe` |
| **PTZCameraOperator.exe** | Main executable (requires DLLs from the portable ZIP to run; prefer installer or ZIP) |

## Updating this repo

From the main [PTZ_Interface](https://github.com/devildog5x5/PTZ_Interface) repo root, run:

```powershell
.\copy-build-to-downloads.ps1
```

Then commit and push the updated files in `PTZCameraOperator-Downloads`.

## Make the main page accessible via external URL (GitHub Pages)

To serve the download page at a public URL:

1. Push this folder to GitHub as its own repo (e.g. **PTZCameraOperator-Downloads**).
2. On GitHub: open the repo → **Settings** → **Pages** (left sidebar).
3. Under **Build and deployment**, set **Source** to **Deploy from a branch**.
4. Choose **Branch:** `main` (or `master`), **Folder:** `/ (root)`, then **Save**.
5. After a minute or two, the main page is live at:
   **https://devildog5x5.github.io/PTZCameraOperator-Downloads/**  
   (Replace `devildog5x5` with your GitHub username if different.)

The installer, portable ZIP, and executable links on the page use relative paths, so they work from that same URL. The `.nojekyll` file in this repo tells GitHub Pages to serve the files as-is (no Jekyll processing).
