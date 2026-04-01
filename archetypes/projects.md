+++
title          = '{{ replace .File.ContentBaseName "-" " " | title }}'
date           = '{{ .Date }}'    # start date — used for default sort order
date_precision = 'month'
draft          = true

# End date — either a date string ("2025-03"), "present", or blank (= present).
# Unlike `date`, Hugo does not parse this automatically, so "present" is safe.
end_date = 'present'

status = 'active'    # active | completed | archived

# Categories become a Hugo taxonomy — browsable at /categories/<term>/.
# Use slugs: lowercase, hyphens, no spaces. e.g. ["machine-learning", "open-source"]
categories = []

# Links
github = ''    # e.g. "https://github.com/you/repo"
demo   = ''    # live demo URL
docs   = ''    # documentation URL

# Arbitrary additional links: [{label = "Paper", url = "https://..."}]
links = []

# Short description shown on the card and in meta description.
abstract = ''
+++

<!-- Full project description in Markdown goes here. -->
