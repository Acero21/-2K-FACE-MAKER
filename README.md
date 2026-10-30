# -2K-FACE-MAKER
Offline NBA 2K20 Cyberface Texture Maker
# 2K FACE MAKER — Android starter build

Offline-first Android starter app for preparing NBA 2K-style texture-map experiments.

## Current MVP features
- Import an image using Android's system file picker
- Preview the selected map (tap a map tab)
- Generate 2048×2048 Diffuse, Normal (estimated), Specular, Face Detail, grayscale Height, and experimental Hair mask maps
- Adjust brightness/contrast and apply edits to the selected map
- Export selected or all PNG maps to `Pictures/2KFaceMaker` and a private app folder
- GitHub Actions workflow to build a debug APK

## Important limitations
This is an early MVP, not the complete feature set. The generators do not yet perform NBA 2K20 UV landmark fitting or reconstruct a true UV texture from multiple camera views. Height and Normal are image-derived approximations; the Hair mask is a basic threshold mask. Tattoo Studio, four-view alignment, project save/reopen UI, layers, and dedicated body UV mapping are not implemented yet. For game use, map the artwork to the correct NBA 2K20 UV template and test it in-game.

## Build on an Android phone
1. Upload the contents of this project folder to a GitHub repository.
2. Open the repository's **Actions** tab.
3. Select **Build 2K Face Maker APK** and tap **Run workflow** (or push to `main`).
4. Open the completed workflow run and download the `2KFaceMaker-debug-apk` artifact.
5. Extract the artifact ZIP and install `app-debug.apk` on your Android phone. Allow installation from that source if Android asks.

