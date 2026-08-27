# HARP Coin

Static landing page for HARP Coin, including its token information, purchase guide, NFT collection links, roadmap and community resources.

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
- Links to the CyberBearz Army (`/cba`), Shit Punks Club (`/spc`) and Squid Gang Club (`/sgc`) static NFT apps
- Whitepaper and audit PDFs in `assets/`

## Project structure

```text
.
├── index.html       # Main landing page
├── css/             # Theme and responsive styling
├── img/             # Brand, content and generated hero assets
├── js/              # Existing site behaviour and live-data formatting
├── assets/          # Whitepaper and audit documents
├── cba/             # CyberBearz Army app
├── spc/             # Shit Punks Club app
└── sgc/             # Squid Gang Club app
```

## Deployment

Deploy the repository root to any static hosting provider. The `/cba`, `/spc` and `/sgc` folders must remain available as static paths because the landing page links directly to them.

## Development notes

- Keep existing external URLs, anchor IDs and the live data endpoint intact when making visual changes.
- The site has no Node.js package manifest or automated build/test scripts.
- Generated hero artwork is stored locally at `img/generated/harp-coin-hero.png`.
