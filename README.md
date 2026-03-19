# InputStats Website

Static website for website-based macOS distribution.

## Files

- `index.html`: download landing page
- `privacy.html`: privacy policy and permissions explanation
- `releases.html`: public release notes
- `downloads/index.html`: download directory landing page
- `downloads/`: published DMG and checksum files
- `updates/appcast.xml`: appcast placeholder
- `styles.css`: shared website styles

## Release flow

1. Build the website test DMG
2. Place the `.dmg` and `.sha256` into `downloads/`
3. Keep a stable copy such as `InputStats-latest.dmg`
4. Update `releases.html`
5. Update `updates/appcast.xml` if you ship in-app updates later
6. Deploy this folder to your website host

## Notes

- This website currently targets `Personal Team` / non-notarized test distribution
- Download instructions should clearly mention `right-click > Open` and the `Privacy & Security` fallback

## Deployment

- GitHub Pages or any static hosting provider
- if using GitHub Pages, keep `.nojekyll`
