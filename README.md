# kevinz-01.github.io

Personal website of Kaiwen Zhou. A small Jekyll site that GitHub Pages builds automatically on push — no theme gem or Actions needed.

## Where to edit

| What | File |
| --- | --- |
| Name, subtitle, email, socials, nav | `_config.yml` |
| Bio and service | `index.html` |
| News | `_data/news.yml` (newest first) |
| Publications | `_data/publications.yml` (`selected: true` → shown on home page) |
| Photo / CV | `images/profile.png`, `files/cv_Kaiwen_Zhou.pdf` |
| Styles | `assets/css/main.css` |

## Preview locally

```bash
docker run --rm -p 4000:4000 -v "$PWD":/srv/jekyll -w /srv/jekyll ruby:3.3 \
  sh -c "bundle install && bundle exec jekyll serve --host 0.0.0.0"
```

Then open http://localhost:4000.
