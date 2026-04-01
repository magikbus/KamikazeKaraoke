# Kamikaze Karaoke Song Search

This folder is ready to publish as a GitHub Pages site.

## Files

- `index.html` - the single-page searchable website
- `songs-data.js` - exported song catalog used by the site
- `Kamikaze_Karaoke_Logo.png` - logo displayed on the page
- `build-site.ps1` - rebuilds `songs-data.js` from the Excel workbook if the song list changes
- `.nojekyll` - tells GitHub Pages to serve the files directly without Jekyll processing

## Rebuild The Song Data

If you update `Kamikaze_Karaoke_Full_Song_List.xlsx`, run:

```powershell
powershell -ExecutionPolicy Bypass -File .\build-site.ps1
```

Then upload or commit the updated `songs-data.js` file to GitHub.

## Publish On GitHub Pages

1. Create a new GitHub repository.
2. Upload `index.html`, `songs-data.js`, `Kamikaze_Karaoke_Logo.png`, and `.nojekyll`.
3. In the repository, open `Settings` > `Pages`.
4. Under `Build and deployment`, set `Source` to `Deploy from a branch`.
5. Select the `main` branch and `/ (root)` folder, then save.
6. Wait for GitHub to publish the site and use the provided public URL.
