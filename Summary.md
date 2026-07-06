# Summary

## What You Just Cloned
- This is the AcademicPages Jekyll theme (Minimal Mistakes derivative) wired for GitHub Pages, so you get turnkey layouts for an academic CV site plus helper scripts for publications, talks, and maps.
- All site-wide knobs live in `_config.yml`, while navigation labels and any future multilingual/UI tweaks live in `_data/`.
- GitHub Pages will build automatically from `main`, but you can preview locally with `bundle install && jekyll serve -l -H localhost`. Docker (`docker compose up`) is pre-configured if you would rather not install Ruby.

## Site-Wide Configuration
- `_config.yml` holds the title, base URL, sidebar bio, social links, default layouts, enabled collections, and global theme (`site_theme: default` vs `air`). Update this first so metadata, feeds, and SEO tags are correct.
- `_data/navigation.yml` defines the order and URLs of the header menu. Add/remove entries to surface or hide sections (e.g., new pages, CV flavor, external links).
- `_data/ui-text.yml` lets you rename built-in UI strings (e.g., "Posts", "Read More") if you want different phrasing.

## Content Buckets You Can Customize
- **Blog posts (`_posts/`)**: Markdown files must follow the `YYYY-MM-DD-title.md` convention with front matter for `title`, `tags`, and optional `permalink`. Draft new ideas in `_drafts/` until you are ready to publish.
- **Standalone pages (`_pages/`)**: Anything from About, CV, Publications, custom landing pages, etc. Give each file front matter with `permalink` and `title`, then link it through `navigation.yml` or inline buttons.
- **Portfolio items (`_portfolio/`)**: Front matter controls teaser text or inline images (see `excerpt` HTML). Markdown or HTML both work, so you can embed figures, slides, or video.
- **Publications (`_publications/`)**: Each file stores venue metadata plus optional `paperurl`, `slidesurl`, and `bibtexurl`. These surface automatically wherever publications are rendered, so you just need to drop PDFs/slides in `files/` and update the URLs.
- **Talks (`_talks/`)** and **Teaching (`_teaching/`)**: Similar front matter-driven pages for seminars/lectures or course entries. You can add `slidesurl`, `video`, or `location` fields to show action buttons and badges.
- **Supporting data**: `files/` exposes uploads at `https://<username>.github.io/files/...` (great for CV PDFs, slides, poster images). `images/` and `assets/` hold static media referenced in posts or CSS.

## Figures, Media, and Slides
- Store figures under `images/` (keep logical subfolders such as `images/research/experiment1.png`). Reference them via standard Markdown (`![caption](/images/...)`) or HTML if you need sizing classes.
- Hero images/backgrounds can also be attached via `header:` front matter on any page/post.
- Upload decks, posters, and datasets to `files/` so you can link using relative URLs; GitHub Pages will serve them verbatim. Use `slidesurl`, `paperurl`, `posterurl`, etc., in front matter wherever you need download buttons.
- Custom fonts/colors: tweak `_sass/` and `assets/css/main.scss` (or switch `site_theme`) for branding; for quick palette changes, override variables in a new partial and import it into `main.scss`.

## Automation Helpers
- `markdown_generator/` contains TSV -> Markdown scripts/notebooks for bulk-importing publications or talks. Update the TSVs with your citation data, run the notebook/script, and copy the generated Markdown into `_publications/` or `_talks/`.
- `talkmap/` + `talkmap.py` can build a leaflet map of your speaking history based on `_talks/` metadata (enable `talkmap_link` in `_config.yml` once you have real data).

## Recommended Adaptation Path
1. Update `_config.yml` with your name, bio, site URL, theme choice, and analytics IDs. Double-check social links and contact info.
2. Rewrite the key `_pages/` content (`about.md`, `cv.md`, `publications.html`, etc.) so each page reflects your research story; hide anything you do not need by removing it from `navigation.yml`.
3. Migrate your blog posts into `_posts/` (or `_drafts/` while editing). Use tags and categories to power the archive pages already wired into the theme.
4. Drop figures into `images/` and slides/posters into `files/`, then reference them via front matter or inline Markdown wherever relevant (portfolio cards, publication entries, talk pages).
5. Add portfolio case studies under `_portfolio/` to highlight projects beyond papers (embed figures/gifs directly in the Markdown to keep things visual).
6. Use the publication/talk generators if you have structured data; otherwise, hand-author Markdown files with the provided examples as templates.
7. Preview locally, iterate on styling (SCSS, theme setting), then push to the `main` branch of `<username>.github.io` to go live.

This repo already mirrors most components you need (blog, CV, publications, course list, talks, portfolio). Treat each folder as a content type, keep media in `images/` or `files/`, and control presentation through front matter plus `_config.yml`.
