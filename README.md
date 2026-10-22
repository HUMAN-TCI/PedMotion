# PedMotion — GitHub Pages Project Website

A static project website featuring eight skeleton animation GIFs and seven SMPL animation GIFs from the supplied **Revision PedWalk.zip**, with mobile-friendly presentation, search/filter controls, a method overview, and reported comparison values.

## Publish in GitHub Pages

1. Create a **public GitHub repository** (for example, `pedmotion-project`).
2. Upload **all the contents of this folder** to the repository's **root** (including `index.html`, `style.css`, `script.js`, `assets/`, and `.nojekyll`). Do **not** upload only the ZIP file.
3. In the repository open **Settings → Pages → Build and deployment**.
4. Select **Deploy from a branch**, branch **main**, folder **/(root)**, then **Save**.
5. Your page will be at `https://YOUR-USERNAME.github.io/pedmotion-project/` once GitHub finishes deployment.

For a `YOUR-USERNAME.github.io` repository, your address is instead `https://YOUR-USERNAME.github.io/`.

## What's included

- 8 skeleton demonstrations (+ one combined overview GIF)
- 7 SMPL demonstrations (the roadside-pickup SMPL example was not supplied)
- Selected manuscript-reported **baseline** numbers (not results of a controlled complete-framework comparison)
- Responsive design, category filters, and motion search

## Add your research links

In `index.html`, search for `Research manuscript` and `Source code`. Replace the placeholder resource rows with your own actual public URLs. Add the exact manuscript title, authors, publication venue, citations and accepted DOI after verification.

## Add the missing SMPL animation

Put `04_roadside_pickup_smpl.gif` inside `assets/smpl/`. In `index.html`, find the card titled **Roadside pickup** and replace its `div class="missing"` with:

```html
<img loading="lazy" src="assets/smpl/04_roadside_pickup_smpl.gif" alt="SMPL animation for roadside pickup" />
```

Then change the `NOT AVAILABLE` text to `ANIMATED` and the SMPL count in the statistic band from 07 to 08.

## Local preview

Open `index.html` directly in your browser. This site does not require npm, Python packages, server-side code, or a build process. For a local server, use `python -m http.server 8000` from this directory and open `http://localhost:8000`.

## Data and claim integrity

The animations in this package are provided example visualizations. We do not claim they are matched baseline comparisons, that any objects are explicitly modeled, or that the reported baseline metrics represent ablations of the entire PedMotion framework. Replace any manuscript summary or reported number if your final published source differs.

## Licensing

No license is included: confirm permissions for paper figures, animations, and model outputs before publicly distributing them. Add a LICENSE file if you want to grant reuse rights.
