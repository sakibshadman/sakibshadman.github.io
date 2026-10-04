# sakibshadman.github.io

Source for my academic homepage: **https://sakibshadman.github.io**

Built with Jekyll on GitHub Pages, using the [AcadHomepage](https://github.com/RayeRen/acad-homepage.github.io) template by Yi Ren (MIT License).

## Where to edit what

| To change… | Edit this file |
|---|---|
| Name, photo, sidebar links, email, CV link | `_config.yml` (the `author:` block) |
| Top navigation bar | `_data/navigation.yml` |
| Bio and research interests | `_pages/includes/intro.md` |
| News | `_pages/includes/news.md` |
| Publications | `_pages/includes/pub.md` |
| Honors, education, experience, teaching, service | `_pages/includes/*.md` |
| Profile photo | replace `images/profile.jpg` (square, ~600×600) |
| Paper thumbnails | replace `images/<name>.png` (5:3, e.g. 1000×600) |
| CV PDF | replace `files/CV-Shadman.pdf` |

Every commit to `main` rebuilds the site automatically in about a minute.

## Citation counts

`.github/workflows/google_scholar_crawler.yaml` runs daily (and on demand from the **Actions** tab). It reads the repository secret `GOOGLE_SCHOLAR_ID` and writes citation data to the `google-scholar-stats` branch, which feeds the citations badge on the homepage.

To show a per-paper count, add this next to a paper, using the ID from the paper's Google Scholar link (`citation_for_view=…`):

```html
<strong><span class='show_paper_citations' data='RlxTPrkAAAAJ:XXXXXXXXXXXX'></span></strong>
```

## Preview locally (optional)

```bash
bundle install
bundle exec jekyll serve
# open http://127.0.0.1:4000
```
