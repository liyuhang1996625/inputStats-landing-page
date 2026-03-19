# InputStats Website

Static website for website-based macOS distribution.

## Files

- `index.html`: download landing page
- `privacy.html`: privacy policy and permissions explanation
- `releases.html`: public release notes
- `updates/appcast.xml`: Sparkle appcast endpoint
- `downloads/`: published DMG and checksum files
- `styles.css`: shared website styles

## Release flow

1. Build and export the notarized macOS app
2. Copy the resulting `.dmg` and `.sha256` into `downloads/`
3. Update `releases.html`
4. Regenerate `updates/appcast.xml`
5. Deploy this folder to your website host

## Deployment

- GitHub Pages or any static hosting provider
- if using GitHub Pages, keep `.nojekyll`
