+++
title          = '{{ replace .File.ContentBaseName "-" " " | title }}'
date           = '{{ .Date }}'    # start date
date_precision = 'month'
draft          = false

organization   = ''
location       = ''

# Path to organisation logo. Either:
#   - a root-relative path: "/images/acme.png"  (file in static/)
#   - a page bundle resource: "acme.png"         (file next to index.md)
# Omit or leave blank for no logo.
logo           = ''

# End date — "present", blank (= present), or a date string "2025-03".
# Partial dates are padded automatically: "2025" → "2025-01-01".
# "present" entries are sorted above all past entries.
end_date       = 'present'

description    = ''
+++

<!-- Optional: bullet points or extended description in Markdown.
     Rendered below the description on the card if present. -->
