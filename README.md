# HARP Coin

Static landing page for HARP Coin, including its token information, purchase guide, roadmap and community resources.

## Run locally

No package install or build step is required. Serve the repository root with any static-file server:

```bash
python3 -m http.server 4173 --bind 127.0.0.1
```

Then open [http://127.0.0.1:4173](http://127.0.0.1:4173).

## What is included

- Responsive HARP Coin landing page (`index.html`)
- Live price, holder, supply and market-cap display from `https://api.harpcoin.co/harp`
- Tokenomics, wallet purchase instructions, FAQ and roadmap
- Whitepaper and audit PDFs in `assets/`

## Project structure

```text
.
├── index.html       # Main landing page
├── css/             # Theme and responsive styling
├── img/             # Brand, content and generated hero assets
├── js/              # Existing site behaviour and live-data formatting
├── assets/          # Whitepaper and audit documents
├── cba/             # Legacy static app bundle
├── spc/             # Legacy static app bundle
└── sgc/             # Legacy static app bundle
```

## Deployment

Deploy the repository root to any static hosting provider.

## Development notes

- Keep existing external URLs, anchor IDs and the live data endpoint intact when making visual changes.
- The site has no Node.js package manifest or automated build/test scripts.
- Generated hero artwork is stored locally at `img/generated/harp-coin-hero.png`.
