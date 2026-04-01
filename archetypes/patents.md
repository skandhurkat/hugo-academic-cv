+++
title          = '{{ replace .File.ContentBaseName "-" " " | title }}'
date           = '{{ .Date }}'
date_precision = 'day'
draft          = true

# List of inventor names — same display rules as publication authors (uses params.author_name for bolding).
# Your name (params.author_name) will be bolded automatically.
authors = []

# Assignee: the legal owner of the patent (company or "Personal")
assignee = ''

# Patent identifiers — one entry per jurisdiction.
# The Google Patents button is constructed from jurisdiction + number.
# Example:
#   identifiers = [
#       { jurisdiction = "US", number = "US11234567B2" },
#       { jurisdiction = "EP", number = "EP3456789A1"}
#   ]
identifiers = []

# Status: granted | pending | abandoned
status = 'granted'

abstract = ''
+++

<!-- Optional: notes, claims summary, or other content in Markdown. -->
