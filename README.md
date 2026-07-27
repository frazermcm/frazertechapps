# frazertechapps

Public documents — privacy policies, terms of use, and support pages — for
apps published by Frazer Tech Apps. Served with GitHub Pages from the `main`
branch root.

**Live site:** https://frazermcm.github.io/frazertechapps/

## Layout

```
index.html              landing page listing the apps
assets/style.css        shared styling (VibeWardrobe brand tokens)
vibewardrobe/
  index.html            legal & support hub
  privacy.html          privacy policy
  terms.html            terms of use
```

One folder per app. To add another app, copy the `vibewardrobe/` folder as a
starting point and add a card to `index.html`.

## URLs for store listings

| Document | URL |
|---|---|
| VibeWardrobe support / hub | https://frazermcm.github.io/frazertechapps/vibewardrobe/ |
| VibeWardrobe privacy policy | https://frazermcm.github.io/frazertechapps/vibewardrobe/privacy.html |
| VibeWardrobe terms of use | https://frazermcm.github.io/frazertechapps/vibewardrobe/terms.html |

These are the URLs referenced by `expo/constants/legal.ts` in the
[rork-vibewardrobe](https://github.com/frazermcm/rork-vibewardrobe) repo, so
keep the paths stable once a build has shipped.

## Enabling Pages

Settings → Pages → Source: "Deploy from a branch" → Branch `main`, folder
`/ (root)`. The `.nojekyll` file stops Jekyll from processing the site.

## Editing

These files are the single source of truth for the legal documents — the app
repos link here rather than keeping their own copies. Update the "Last
updated" date at the top of a document whenever its content changes
materially.
