+++
title = 'Attention is all you need'
date = '2017-12-01'
draft = false

# List of author names, exactly as you want them displayed.
# Your own name (matching params.author_name) will be bolded automatically.
authors = ["Ashish Vaswani", "Noam Shazeer", "Niki Parmar", "Jakob Uszkoreit", "Llion Jones", "Aidan N Gomez", "Łukasz Kaiser", "Illia Polosukhin"]

# Free-form venue string. Examples:
#   "NeurIPS 2024"
#   "Nature, vol. 42, pp. 1–10"
#   "arXiv preprint"
# Leave blank for books or theses where booktitle/institution is more natural.
venue = 'Advances in Neural Information Processing Systems 30 (NIPS 2017)'

# For book chapters only: the title of the containing book.
booktitle = ''

# Publication type(s). Use a list — a paper can be both 'conference' and
# 'preprint' if it was posted to arXiv before acceptance.
# Valid values: conference, journal, preprint, thesis, book, bookchapter, other
publication_types = ["conference", "preprint"]

# --- Links ---
# doi:   just the identifier, e.g. "10.1145/1234567.1234568"
#        renders as a button linking to https://doi.org/<doi>
# arxiv: just the arXiv ID, e.g. "2401.00000"
#        renders as a button linking to https://arxiv.org/abs/<id>
# pdf:   one of:
#          - a full URL:            "https://example.com/paper.pdf"
#          - a root-relative path:  "/papers/mypaper.pdf"
#          - a page bundle file:    "paper.pdf"  (place file next to index.md)
doi = '10.48550/arXiv.1706.03762'
arxiv = '1706.03762'
pdf = 'https://proceedings.neurips.cc/paper_files/paper/2017/file/3f5ee243547dee91fbd053c1c4a845aa-Paper.pdf'

# Abstract. Hugo TOML supports multiline strings with triple quotes:
#   abstract = """
#   First paragraph.
#
#   Second paragraph.
#   """
abstract = """The dominant sequence transduction models are based on complex
recurrent orconvolutional neural networks in an encoder and decoder
configuration. The best performing such models also connect the encoder and
decoder through an attentionm echanisms. We propose a novel, simple network
architecture based solely onan attention mechanism, dispensing with recurrence
and convolutions entirely.Experiments on two machine translation tasks show
these models to be superiorin quality while being more parallelizable and
requiring significantly less timeto train. Our single model with 165 million
parameters, achieves 27.5 BLEU onEnglish-to-German translation, improving over
the existing best ensemble result by over 1 BLEU. On English-to-French
translation, we outperform the previoussingle state-of-the-art with model by 0.7
BLEU, achieving a BLEU score of 41.1."""

# BibTeX fields used for the auto-generated BibTeX export.
volume      = ''
number      = ''
pages       = ''
publisher   = ''
institution = ''   # for theses
+++
