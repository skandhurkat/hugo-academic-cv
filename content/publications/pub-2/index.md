+++
title = 'Language Models are Few-Shot Learners'
date = '2020-05-28'
draft = false

# List of author names, exactly as you want them displayed.
# Your own name (matching params.author_name) will be bolded automatically.
authors = ["Tom B. Brown", "Benjamin Mann", "Nick Ryder", "Melanie Subbiah", "Jared Kaplan", "Prafulla Dhariwal", "Arvind Neelakantan", "Pranav Shyam", "Girish Sastry", "Amanda Askell", "Sandhini Agarwal", "Ariel Herbert-Voss", "Gretchen Krueger", "Tom Henighan", "Rewon Child", "Aditya Ramesh", "Daniel M. Ziegler", "Jeffrey Wu", "Clemens Winter", "Christopher Hesse", "Mark Chen", "Eric Sigler", "Mateusz Litwin", "Scott Gray", "Benjamin Chess", "Jack Clark", "Christopher Berner", "Sam McCandlish", "Alec Radford", "Ilya Sutskever", "Dario Amodei"]

# Free-form venue string. Examples:
#   "NeurIPS 2024"
#   "Nature, vol. 42, pp. 1–10"
#   "arXiv preprint"
# Leave blank for books or theses where booktitle/institution is more natural.
venue = ''

# For book chapters only: the title of the containing book.
booktitle = ''

# Publication type(s). Use a list — a paper can be both 'conference' and
# 'preprint' if it was posted to arXiv before acceptance.
# Valid values: conference, journal, preprint, thesis, book, bookchapter, other
publication_types = ["preprint"]

# --- Links ---
# doi:   just the identifier, e.g. "10.1145/1234567.1234568"
#        renders as a button linking to https://doi.org/<doi>
# arxiv: just the arXiv ID, e.g. "2401.00000"
#        renders as a button linking to https://arxiv.org/abs/<id>
# pdf:   one of:
#          - a full URL:            "https://example.com/paper.pdf"
#          - a root-relative path:  "/papers/mypaper.pdf"
#          - a page bundle file:    "paper.pdf"  (place file next to index.md)
doi   = ''
arxiv = ''
pdf   = 'pdf.txt'

# Abstract. Hugo TOML supports multiline strings with triple quotes:
#   abstract = """
#   First paragraph.
#
#   Second paragraph.
#   """
abstract = """Recent work has demonstrated substantial gains on many NLP tasks
and benchmarks by pre-training on a large corpus of text followed by fine-tuning
on a specific task. While typically task-agnostic in architecture, this method
still requires task-specific fine-tuning datasets of thousands or tens of
thousands of examples. By contrast, humans can generally perform a new language
task from only a few examples or from simple instructions - something which
current NLP systems still largely struggle to do. Here we show that scaling up
language models greatly improves task-agnostic, few-shot performance, sometimes
even reaching competitiveness with prior state-of-the-art fine-tuning
approaches. Specifically, we train GPT-3, an autoregressive language model with
175 billion parameters, 10x more than any previous non-sparse language model,
and test its performance in the few-shot setting. For all tasks, GPT-3 is
applied without any gradient updates or fine-tuning, with tasks and few-shot
demonstrations specified purely via text interaction with the model. GPT-3
achieves strong performance on many NLP datasets, including translation,
question-answering, and cloze tasks, as well as several tasks that require
on-the-fly reasoning or domain adaptation, such as unscrambling words, using a
novel word in a sentence, or performing 3-digit arithmetic. At the same time, we
also identify some datasets where GPT-3's few-shot learning still struggles, as
well as some datasets where GPT-3 faces methodological issues related to
training on large web corpora. Finally, we find that GPT-3 can generate samples
of news articles which human evaluators have difficulty distinguishing from
articles written by humans. We discuss broader societal impacts of this finding
and of GPT-3 in general."""

# BibTeX fields used for the auto-generated BibTeX export.
volume      = ''
number      = ''
pages       = ''
publisher   = ''
institution = ''   # for theses
+++
