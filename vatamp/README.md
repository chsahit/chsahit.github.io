# VA-TAMP project website

Project page for *Visibility-Aware Task and Motion Planning with Task-Centric Perception*
(submitted to ICRA 2027), built on the [Nerfies](https://github.com/nerfies/nerfies.github.io) template.

## Layout

- `index.html` — the whole page.
- `static/vatamp_paper.pdf` — paper compiled with review notes off (`\ReviewNotesMode{off}`).
- `static/images/` — Fig. 1 panels, Fig. 2 (cropped from the compiled PDF), Fig. 3 (PCF), task scenes.
- `static/videos/` — clips cut from `vatamp_video_FINAL_icra.mp4` plus per-run robot videos
  (re-encoded to H.264, ~15 MB total).

## Before publishing

- Replace `Anonymous Authors` and the affiliation line in the hero, and the BibTeX entry.
- Uncomment the arXiv / Code buttons in the hero once links exist.
- Make the `og:image` / `twitter:image` meta tags absolute URLs (e.g. `https://<site>/static/images/thumbnail.png`); social previews ignore relative paths.
- If the paper PDF changes, re-copy it to `static/vatamp_paper.pdf` and re-crop Fig. 2
  (`static/images/method_overview.png`) from page 2 at 300 dpi.

## Preview locally

```
python3 -m http.server 8000
# open http://localhost:8000
```
