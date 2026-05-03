# Hugo Theme: Academic CV

This is a simple academic CV style theme for [Hugo](//gohugo.io). It is
meant to be a lightweight replacement for the hugo-academic theme by
[gcushen](//github.com/gcushen)
([forked here](//github.com/skandhurkat/hugo-academic) and now
[lives as a HugoBlox/Netlify theme](//github.com/HugoBlox/hugo-theme-academic-cv)).
This is a clean-room implementation that is meant to provide a similar
appearance and functionality, while minimizing third-party dependencies
and feature bloat.

You may view a preview of this theme on [my website](//skandhurkat.com).

## Features

- Academic CV with sections for
  - bio
  - experience
  - publications
  - patents
  - projects
  - blog posts
  - contact information

- Automatic sort
  - experience by end date
  - publications, patents, projects, and blog posts by publication date

- Client-side javascript filtering of
  - publications by type (conference, journal, preprint, etc.)
  - patents by status (granted, pending, expired)
  - projects by tags

- JSON-LD for SEO

- Client-side search using [Fuse.js](//www.fusejs.io).

## Installing

Clone this theme as a submodule in your website's `themes/` folder

```bash
git clone https://github.com/skandhurkat/hugo-theme-academic-cv themes/academic-cv
```

Then, modify your site's `hugo.toml` to point to the new theme and to
configure it:

```toml
baseURL        = 'https://example.com'
locale         = 'en-US'
title          = 'Example Site'
theme          = 'academic-cv'

# ---------------------------------------------------------------------------
# Taxonomies
# Hugo requires you to list ALL taxonomies you want, including any you want
# to keep from the defaults (tags, categories). Format: singular = 'plural'.
# The plural form becomes the URL: /publication_types/conference/
# ---------------------------------------------------------------------------
[taxonomies]
  tag              = 'tags'
  publication_type = 'publication_types'
  category         = 'categories'

# ---------------------------------------------------------------------------
# Navigation menu
# pageRef is a root-relative path to the section. Hugo resolves it to the
# section's _index.md. weight controls the order (lower = further left).
# ---------------------------------------------------------------------------
[menus]
  [[menus.main]]
    name    = 'Experience'
    pageRef = '/experience'
    weight  = 10
  [[menus.main]]
    name    = 'Publications'
    pageRef = '/publications'
    weight  = 20
  [[menus.main]]
    name    = 'Patents'
    pageRef = '/patents'
    weight  = 30
  [[menus.main]]
    name    = 'Projects'
    pageRef = '/projects'
    weight  = 40
  [[menus.main]]
    name    = 'Posts'
    pageRef = '/posts'
    weight  = 50
  [[menus.main]]
    name    = 'Contact'
    url     = "/#contact"
    weight  = 60

# ---------------------------------------------------------------------------
# Theme parameters
# All of these are available in templates as site.Params.<key>.
# Provide sensible defaults here; users override in their site's hugo.toml.
# ---------------------------------------------------------------------------
[params]
  # --- Identity ---
  # author_name is used in two places:
  #   1. author_list.html bolds your name in author lists
  #   2. JSON-LD Person schema (later)
  author_name  = "Example Site"
  author_title = "Example Position"
  author_email = "example@example.com"

  # --- Homepage section limits ---
  # How many items to show in each homepage hero section before "see all".
  home_publications_count = 3
  home_patents_count      = 3
  home_posts_count        = 4
  home_projects_count     = 3
  home_experience_count   = 4

  # --- Integrations (leave blank to disable) ---
  cookie_consent   = true

  google_analytics = ""   # e.g. "G-XXXXXXXXXX"
  disqus_shortname = ""   # e.g. "mysite"

  # --- Dark mode ---
  # "auto"  = respect the OS prefers-color-scheme setting
  # "light" = always light
  # "dark"  = always dark
  dark_mode = "auto"

  favicon = ""

  # --- Publication type accent colours ---
  # These feed into CSS custom properties via Hugo Pipes (see assets/css/main.css).
  # You can override any or all of these in your site's hugo.toml.
  # Values are any valid CSS colour: hex, rgb(), hsl(), etc.
  [params.pub_colors]
    conference   = "#378ADD"
    journal      = "#1D9E75"
    preprint     = "#EF9F27"
    thesis       = "#7F77DD"
    book         = "#D85A30"
    bookchapter  = "#D85A30"   # same family as book
    other        = "#888780"
```
