# CinarogluLab Website

Source of <https://cinaroglulab.github.io/>, the site of the Laboratory for Molecular Modeling & Drug Discovery at Ege University. GitHub Pages builds it with Jekyll on every push to `main`.

## Updating content

Almost every edit is a YAML file in `_data/`:

| File | What it holds |
|------|---------------|
| `_data/news.yml` | News items (newest first) |
| `_data/publications.yml` | Highlighted publications |
| `_data/team.yml` | PI and students |
| `_data/research.yml` | Research areas (home cards and research page) |
| `_data/methods.yml` | "Our methodologies" list on the home page |
| `_data/vacancies.yml` | Open positions and how to apply |
| `_data/software.yml` | Software links |
| `_data/partners.yml` | Affiliation logos in the footer band |
| `_data/navigation.yml` | Top and footer menu |

Images go in `images/` (`teampic/`, `pubpic/`, `logopic/`); reference them by file name in the YAML.

## Layout

```
_config.yml        site settings
_data/             content (see above)
_includes/         head, header, footer, partner band, frame corners
_layouts/default   the one page layout
_pages/            one file per page: home, research, team, publications, vacancies, software, news, 404
css/main.css       all styles (plain CSS, design tokens at the top)
fonts/             self-hosted Barlow / Barlow Condensed
images/            photos and figures
```

## Preview locally

```sh
bundle install
bundle exec jekyll serve
```

Then open <http://localhost:4000>.

The original template came from [allanlab](https://github.com/mpa139/allanlab). Content © CinarogluLab, MIT License.
