<!-- rebuild trigger -->
# Website of the CS2Italy conference

GitHub Pages builds the entire site from `docs/` with `docs/_config.yml`.
The home page is the current edition (being prepared for 2027; it still shows
the Torino 2026 content until it is updated). Past editions are archived at
`/2026/` (Torino) and `/2025/` (Trento).

Each archive uses its own layout, `docs/_layouts/<year>.html`, and its own
metadata and CSV tables in `docs/_data/<year>/` (`conference.yml` holds the
fields that `docs/_config.yml` provides for the current edition). Its text and
assets stay in `docs/<year>/`. Jekyll only loads layouts, data, and build
settings from the site root, so archived editions must not rely on nested
`_layouts`, `_data`, or `_config.yml` files.

To archive the current edition at the end of a year, copy `docs/assets/` and
`docs/_texts/` into `docs/<year>/`, the CSV tables into `docs/_data/<year>/`,
the edition fields of `docs/_config.yml` into `docs/_data/<year>/conference.yml`,
and `docs/_layouts/default.html` into `docs/_layouts/<year>.html`. In the new
layout, read `site.data.<year>` and its `conference` entry instead of
`site.data` and `site`, and point every asset link to `/<year>/assets/`. Then
add `docs/<year>/index.md` with `layout: "<year>"` and `permalink: /<year>/`.

To preview all editions, run `bundle install` and `bundle exec jekyll serve`
from `docs/`, then open `/`, `/2026/` and `/2025/` on the local preview server.
