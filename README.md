# The Lamplighter

A sleep-onset story game for the browser. You are the village lamplighter:
two hundred lamps between the bakery and the far edge of the parish, five
maps, thirty-six kinds of small slow task — and no score, no failure, no
time pressure. The night dims as you play, and if you drift off for five
minutes, the round ends itself. Built on sleep research (cognitive
shuffling / serial diverse imagining, low-arousal game design).

**Play it, in bed, with your screen brightness all the way down.**

## Publish on GitHub Pages

1. Create a new repository (e.g. `lamplighter`).
2. Upload the contents of this folder (`index.html`, `.nojekyll`, `README.md`).
3. Repo **Settings → Pages → Build and deployment**: Source = *Deploy from a
   branch*, Branch = `main`, folder = `/ (root)`. Save.
4. Your game is live at `https://<username>.github.io/lamplighter/` within a
   minute or two.

(Alternately: name the repo `<username>.github.io` and it serves at the root.)

## Notes

- Everything is one file — no build step, no dependencies to install.
- The character in Customize ALWAYS shows: a built-in animated 2D preview
  renders instantly with zero network. The rotatable 3D version upgrades in
  automatically when Three.js loads — it tries a local `three.min.js` beside
  `index.html` first, then three CDNs (cdnjs, jsDelivr, unpkg).
- Optional, for 3D with no network at all: download
  https://cdn.jsdelivr.net/npm/three@0.128.0/build/three.min.js
  and commit it next to `index.html` as `three.min.js`. Done — fully
  self-hosted, no CDN involved.
- Progress, fireflies, wardrobe and achievements save in the browser's
  localStorage — same browser, same device. Clearing site data erases the save.
- Sound starts after the first tap (browser autoplay rules). Spoken narration
  uses the browser's speech synthesis where available.
