# gswagel.github.io

Personal academic website for Gabriel Swagel, served at
<https://gswagel.github.io>. Built with [Jekyll](https://jekyllrb.com/) on the
[academicpages](https://github.com/academicpages/academicpages.github.io)
template (a fork of [Minimal Mistakes](https://mmistakes.github.io/minimal-mistakes/))
and deployed via GitHub Pages.

## Editing content

| What | Where |
|------|-------|
| Bio / home page | `_pages/about.md` |
| Publications & working papers | `_publications/*.md` (one file per paper) |
| CV page | `_pages/cv.md` |
| CV PDF, paper PDFs | `files/` |
| Headshot | `images/profile.jpg` |
| Sidebar (name, bio, email, links) | `author:` block in `_config.yml` |
| Header navigation | `_data/navigation.yml` |

Each publication's `category:` (`published` or `working_papers`) controls which
heading it appears under on the Publications page; the heading labels live under
`publication_category:` in `_config.yml`.

## Building locally (Windows)

Requires Ruby + DevKit (installed via `winget install RubyInstallerTeam.RubyWithDevKit.3.3`).

```powershell
bundle install              # first time only
bundle exec jekyll serve -l -H localhost
```

Then open <http://localhost:4000>. The site rebuilds on save (except
`_config.yml`, which needs a server restart).

## Deploying

Push to `main`. GitHub Pages rebuilds and publishes automatically (Settings →
Pages → Build and deployment → *Deploy from a branch* → `main` / `/ (root)`).
