+++
title   = '{{ replace .File.ContentBaseName "-" " " | title }}'
date    = '{{ .Date }}'
draft   = true

# List of author names, exactly as you want them displayed.
# Your own name (matching params.author_name) will be bolded automatically.
authors = []

# Free-form venue string. Examples:
#   "NeurIPS 2024"
#   "Nature, vol. 42, pp. 1–10"
#   "arXiv preprint"
venue = ''

# For book chapters only: the title of the containing book.
booktitle = ''

# Publication type(s). Use a list — a paper can be both 'conference' and
# 'preprint' if it was posted to arXiv before acceptance.
# Valid values: conference, journal, preprint, thesis, book, bookchapter, other
publication_types = []

# Date precision controls how the date is displayed.
# Hugo always needs a full date internally, so if you only know the year,
# set date = '2024-01-01' and date_precision = 'year'.
# Options: "year" | "month" | "day"   — default is "month" if omitted.
date_precision = 'month'

# --- Links ---
# doi:   just the identifier, e.g. "10.1145/1234567.1234568"
# arxiv: just the arXiv ID, e.g. "2401.00000"
# pdf:   URL, root-relative path, or page bundle filename
doi   = ''
arxiv = ''
pdf   = ''

# Abstract. Supports multiline TOML strings:
#   abstract = """
#   First paragraph.
#
#   Second paragraph.
#   """
abstract = ''

# BibTeX metadata — used for the auto-generated BibTeX export.
# These are optional; omit any that don't apply.
volume      = ''
number      = ''
pages       = ''
publisher   = ''
institution = ''   # for theses
+++

<!-- Optional: full paper content in Markdown goes here.
     This appears on the single publication page below the abstract.
     Leave blank if you just want the metadata + links. -->
