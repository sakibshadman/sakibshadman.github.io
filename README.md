# Shadman Sakib — Academic Personal Website

Source for my academic homepage: **https://sakibshadman.github.io/**

The site presents my research, publications, academic experience, honors and
awards, teaching, and professional service. It is built with Jekyll and hosted
on GitHub Pages; every commit to `main` rebuilds it in about a minute.


## Where to edit what

| To change… | Edit |
|---|---|
| Name, photo, affiliation, email, CV link | `_config.yml` (the `author:` block) |
| Top navigation bar | `_data/navigation.yml` |
| News items | `_data/news.yml` |
| Bio and research interests | `_pages/includes/intro.md` |
| Upcoming travel and talks | `_includes/upcoming-panel.html` |
| Research highlights and publications | `_pages/includes/pub.md` |
| Honors, education, experience, teaching, service | `_pages/includes/*.md` |
| Which sections appear, and in what order | `_pages/about.md` |
| Colours, spacing, every component | `assets/css/main.scss` |
| Profile photo | replace `images/profile.jpg` (square, ~600×600) |
| Paper thumbnails | replace `images/<name>.png` |
| Link preview card | replace `images/social-card.png` (1200×630) |
| CV PDF | replace `files/CV-Shadman.pdf` |


## Layout

- `_layouts/default.html` — the page shell
- `_includes/` — sidebar, top bar, news panel, upcoming panel, footer
- `_sass/` — the theme's base styles; site-specific styles live at the end of
  `assets/css/main.scss`


## Citation counts

The sidebar citation line reads `gs_data.json` from the `google-scholar-stats`
branch and stays hidden until that branch exists. Google Scholar usually refuses
GitHub's servers, so the data is refreshed from a local machine:

```bash
python3 -m venv .venv && source .venv/bin/activate
pip install -r google_scholar_crawler/requirements.txt
python google_scholar_crawler/run_locally.py
```


## Preview locally (optional)

```bash
bundle install
bundle exec jekyll serve
# open http://127.0.0.1:4000
```


## Acknowledgements

This website is based on and adapted from **AcadHomepage**, developed by
**Yi Ren (RayeRen)**:

https://github.com/RayeRen/rayeren.github.io

The original AcadHomepage project is distributed under the MIT License.

AcadHomepage itself incorporates or is influenced by several open-source
projects, including:

- Font Awesome
- Minimal Mistakes
- Academic Pages

I gratefully acknowledge the developers and contributors of these projects for
making their work publicly available.


## License

The portions of this repository derived from AcadHomepage remain subject to the
original MIT License and copyright notice.

Copyright (c) 2022 Yi Ren

My personal content — biography, research descriptions, publications, images and
other original materials — belongs to their respective author(s) unless
otherwise stated.
