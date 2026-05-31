# Academis Demo

Live showcase of the [Academis Hugo theme](https://github.com/critoracy/Academis).

**Live site:** https://critoracy.github.io/academis-demo/

## Features demonstrated

| Section | URL | Features |
|---------|-----|----------|
| Home | `/` | Article feed + sections explore |
| Standard article | `/articole/standard/` | Read layout, eyebrow arrow, cover image |
| Academic article | `/articole/academic/` | Metadata box: venue, coauthors, DOI, external URL |
| Portfolio article | `/articole/portfolio/` | Metadata box: role, organization, period |
| Announcements | `/anunturi/` | Glance-list layout, smart search (#tag @status $year), modal fetch |
| Personal feed | `/personal/` | Social-feed layout, mixed post types (text/review/photos), pinned posts |
| CV | `/cv/` | Data-driven CV from `data/cv.yaml` |
| Book | `/carte/` | Book layout, chapter navigation, prev/next |

## Content structure

```
content/
├── articole/       → Read layout (standard, academic, portfolio)
├── anunturi/       → Glance layout (status: active/upcoming/archived)
├── personal/       → Social feed (postKind: text/review/photos)
├── cv/             → CV layout (data from data/cv.yaml)
└── carte/          → Book layout with chapter navigation
```

## Consuming Academis

This site uses `Academis` as a Hugo module:

```toml
# config/_default/hugo.toml
[module]
  [[module.imports]]
    path = "github.com/critoracy/Academis"
```

```
# go.mod
require github.com/critoracy/Academis v0.0.0-...
```
