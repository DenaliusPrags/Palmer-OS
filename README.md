# Palmer OS

Personal life dashboard for Garry Palmer.

## Setup

This is a static PWA. To deploy on GitHub Pages:

1. Push this repository to GitHub
2. Go to Settings → Pages → Source → Deploy from branch → main → / (root)
3. Wait ~60 seconds for deployment
4. Visit `https://yourusername.github.io/palmer-os`
5. On Android Chrome: three-dot menu → Add to Home Screen

## Security

- All data stored locally in browser localStorage — nothing sent to any server except AI planning queries to Anthropic API
- AI planning uses the Anthropic API via the Claude artifact proxy — no API key stored anywhere
- Security headers set in `_headers` file
- Service worker caches assets for offline use

## Files

- `index.html` — The full app
- `manifest.json` — PWA manifest for installability  
- `sw.js` — Service worker for offline support
- `icon-192.png` / `icon-512.png` — App icons
- `_headers` — Security headers (Netlify) / use `_config.yml` for GitHub Pages headers
