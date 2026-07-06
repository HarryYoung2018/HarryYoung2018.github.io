# harryyoung2018.github.io

Personal academic website of **Yonghan (Harry) Yang** — an AI researcher at MBZUAI working on
generative models, agents, and AI for science.

🌐 **Live site:** <https://harryyoung2018.github.io/>

## Sections

- **Home** — bio, research interests, and news
- **Research** (`/publications/`) — papers and manuscripts in progress
- **Projects** (`/portfolio/`) — research & engineering projects
- **Blog** (`/year-archive/`) — notes on mathematics, learning, and life
- **CV** (`/cv/`) — full CV, with a downloadable [PDF](files/Yonghan-Yang-CV.pdf)

## Built with

This site is built with [Jekyll](https://jekyllrb.com/) on the
[Academic Pages](https://github.com/academicpages/academicpages.github.io) template (a fork of
[Minimal Mistakes](https://github.com/mmistakes/minimal-mistakes)) and hosted on GitHub Pages.

### Content lives in

| Directory        | What goes there                          |
| ---------------- | ---------------------------------------- |
| `_pages/`        | Standalone pages (About, CV, Research, Projects) |
| `_publications/` | One Markdown file per paper / manuscript |
| `_portfolio/`    | One Markdown file per project            |
| `_posts/`        | Blog posts (`YYYY-MM-DD-title.md`)       |
| `_config.yml`    | Site-wide settings, sidebar, social links |
| `images/`, `files/` | Media and downloadable assets (CV PDF, figures) |

### Run locally

```bash
bundle install
bundle exec jekyll serve -l -H localhost
# open http://localhost:4000
```

The original template documentation is preserved in
[`README-academicpages.md`](README-academicpages.md), and a customization guide in
[`Summary.md`](Summary.md).

## License

Site content © Yonghan Yang. The underlying Academic Pages / Minimal Mistakes template is
distributed under the MIT License (see [`LICENSE`](LICENSE)).
