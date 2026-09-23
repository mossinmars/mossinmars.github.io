# MOSS / MARSCOIN landing page draft

A static Astro page prepared for GitHub Pages. The X banner is used only as the social preview image; the landing-page hero is a separately generated MOSS scene, based on the supplied portrait.

## Design direction

- **Visual thesis:** MOSS's final frame gives way to a full charge and a blue Martian sunset over his new search.
- **Content plan:** MOSS introduction → battery reaches zero → MarsCoin restores him → his new search → planned dividends → launch coordinates.
- **Interaction thesis:** A gentle hero drift and scroll reveals. Motion is disabled for reduced-motion preferences.

## Run and deploy

```sh
npm install
npm run build
```

The build creates `dist/`. After changing the MOSS GitHub username to `mossinmars`, push the source to the account's `mossinmars.github.io` repository. The workflow in `.github/workflows/deploy.yml` builds and publishes the site through GitHub Pages at `https://mossinmars.github.io/`.

## Story artwork

- [`moss-recharged.png`](public/assets/moss-recharged.png) is the supplied 100% power frame, used as the story section's background.
- [`moss-finds-marscoin-blue-sunset.png`](public/assets/moss-finds-marscoin-blue-sunset.png) is the revised MOSS discovery scene, with the MarsCoin in the marked foreground position and blue twilight around the setting Sun.
- [`marscoin-official-icon.png`](public/assets/marscoin-official-icon.png) is the icon served by [MarsCoin's website](https://www.marscoinbnb.com/assets/marscoin-official-icon.png). The site also renders it separately in HTML for a direct link to MarsCoin.
- The 2.5% volume examples are illustrative total pool calculations, not individual holder payouts.

## Before launch

1. Confirm Flap accepts MarsCoin contract `0xfe189e97832da1573e4e4ff034f4ffc3a15c7777` as the MOSS quote/payment token, and confirm the actual dividend token and distribution on-chain.
2. Confirm the planned holder distribution and how Flap's protocol fee affects it before claiming an exact realized percentage.
3. Replace the disabled Buy button and `TO BE ANNOUNCED` contract with the actual MOSS token address, Flap trading URL, chart, and X account.
4. Confirm the exact banner typeface or supply a font file. The draft uses Michroma as a close display-font stand-in, plus DM Sans for readable body text.
5. If a true interactive 3D MOSS is commissioned later, use a properly modeled and optimized GLB. The current draft uses the provided portrait with lightweight effects.

See [research.md](research.md) for the source-backed context behind the page copy.
