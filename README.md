# Terrain Analysis Tool (phone)

Bohn Ag Consulting. An installable phone/tablet version of the Terrain Analysis Tool: LiDAR elevation, drainage, slope and water analysis that runs entirely on the device.

## Install on iPhone
1. Open the app link in **Safari**.
2. Tap **Share** → **Add to Home Screen** → **Add**.
3. Open **Terrain** from the home screen. Once it has opened, it works offline.

Elevation files (`.tif`, or a `.zip` containing them) are opened from the Files app. Nothing is uploaded.

### Files from Google Drive
The Google Drive app treats a `.tif` as a picture: **Download** saves it to Photos, which ruins it. Instead:
- In Drive, tap **⋯** on the file → **Open in** → **Save to Files**, then open it from Files; or
- keep the elevation files **zipped** in Drive (Clip Zip Ship downloads already are). A `.zip` stays a normal file, and the app opens the `.tif` inside it directly.

## Good to know
- **Reopen**: the last map is kept on the phone; the start screen has a one-tap button to reopen it.
- **Large files** are opened at lower detail (every 2nd or 3rd pixel) so they fit in the phone's memory. A badge under the file name and File information (the **i** button) show the detail used.
- **My location** (arrow button): shows a blue dot where you are. The first time, iPhone asks for permission. If it was refused: Settings › Privacy & Security › Location Services.
- **Pictures and drainage CSVs** open the share sheet: Save to Files, Messages, Mail, etc.

## Updating
Bump `CACHE` in `sw.js` and `APP_VERSION` in `index.html` (same number) whenever you publish changes. Installed copies pick the new version up the next time they are opened with a signal. The version shows on the start screen.
