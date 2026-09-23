# MOSS / MARSCOIN landing page draft

A static Astro page prepared for GitHub Pages. The X banner is used only as the social preview image; the landing-page hero is a separately generated MOSS scene, based on the supplied portrait.

## Design direction

- **Visual thesis:** Warm Mars daylight gives way to MOSS's dark final frame, then a cyan reboot signal.
- **Content plan:** MOSS introduction → battery reaches zero → MarsCoin restores him → his new search → planned dividends → launch coordinates.
- **Interaction thesis:** A gentle hero drift, scroll reveals, and a battery meter that fills when the blackout scene enters view. Motion is disabled for reduced-motion preferences.

## Run and deploy

```sh
npm install
npm run build
```

The build creates `dist/`. After changing the MOSS GitHub username to `mossinmars`, push the source to the account's `mossinmars.github.io` repository. The workflow in `.github/workflows/deploy.yml` builds and publishes the site through GitHub Pages at `https://mossinmars.github.io/`.

## Story artwork

- [`moss-blackout.png`](public/assets/moss-blackout.png) is the supplied frame of MOSS at the moment his power goes out, used as the story section's background.
- [`moss-discovers-marscoin.png`](public/assets/moss-discovers-marscoin.png) was made with the built-in image-generation tool using the supplied MOSS portrait and the existing MOSS hero as references. Prompt: "MOSS alone on a vast Mars plain discovers a small unmarked metallic artifact half buried in red dust. His eyes look down at it with curiosity; his cyan rover light catches its edge. Compose a cinematic wide scene with MOSS on the right, dark mauve sky and uncluttered left space for live typography. Preserve the cream square rover head, blue eyes, cyan mouth light, rusty body, solar panels, and wheels. No emblem, lettering, icon, coin branding, or UI."
- [`marscoin-official-icon.png`](public/assets/marscoin-official-icon.png) is the actual icon served by [MarsCoin's website](https://www.marscoinbnb.com/assets/marscoin-official-icon.png). It is rendered separately in HTML so its identity is not altered by image generation.

## Before launch

1. Confirm Flap accepts MarsCoin contract `0xfe189e97832da1573e4e4ff034f4ffc3a15c7777` as the MOSS quote/payment token, and confirm the actual dividend token and distribution on-chain.
2. Confirm the planned holder distribution and how Flap's protocol fee affects it before claiming an exact realized percentage.
3. Replace the disabled Buy button and `TO BE ANNOUNCED` contract with the actual MOSS token address, Flap trading URL, chart, and X account.
4. Confirm the exact banner typeface or supply a font file. The draft uses Michroma as a close display-font stand-in, plus DM Sans for readable body text.
5. If a true interactive 3D MOSS is commissioned later, use a properly modeled and optimized GLB. The current draft uses the provided portrait with lightweight effects.

See [research.md](research.md) for the source-backed context behind the page copy.
