# PTZ Camera Operator — Downloads

This repository hosts the **download page** for [PTZ Camera Operator](https://github.com/devildog5x5/PTZ_Interface). The page links to the main repo’s [Releases](https://github.com/devildog5x5/PTZ_Interface/releases/latest) for the installer and portable ZIP (GitHub’s 100 MB file limit prevents storing them here).

- **Live download page:** [https://devildog5x5.github.io/PTZCameraOperator-Downloads/](https://devildog5x5.github.io/PTZCameraOperator-Downloads/)
- **Source repo:** [PTZ_Interface](https://github.com/devildog5x5/PTZ_Interface)

## What’s on the page

| Link | Points to |
|------|------------|
| **Windows installer** | PTZ_Interface → `PTZCameraOperatorSetup.exe` |
| **Portable ZIP** | PTZ_Interface → `PTZCameraOperator-Portable.zip` |
| **Executable** | Same portable ZIP (run `PTZCameraOperator.exe` after extracting) |

## GitHub Pages

Pages is already enabled: **Deploy from branch** → **main** → **/ (root)**. The `.nojekyll` file ensures static files are served as-is.

## Updating the page

To change copy or layout, edit `index.html` in this repo and push.  
To publish a new build, create a release in [PTZ_Interface](https://github.com/devildog5x5/PTZ_Interface) (e.g. run `.\publish-release.ps1 -Tag v1.0.1` from that repo). The download page will then serve the new assets automatically.
