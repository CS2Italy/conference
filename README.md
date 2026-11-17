<!-- rebuild trigger -->
# Website of the CS2Italy conference 2026

GitHub Pages builds the entire site from `docs/` with `docs/_config.yml`.
The home page is the Torino 2026 edition; `/2025/` is the Trento archive.

The archive uses `docs/_layouts/2025.html` and its own metadata and CSV tables
in `docs/_data/2025/`. Its text and assets stay in `docs/2025/`. Jekyll only
loads layouts, data, and build settings from the site root, so archived editions
must not rely on nested `_layouts`, `_data`, or `_config.yml` files.

To preview both editions, run `bundle install` and `bundle exec jekyll serve`
from `docs/`, then open `/` and `/2025/` on the local preview server.
