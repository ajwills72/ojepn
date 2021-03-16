# OJEPN production pipeline

## Process overview

1. Paper as single PDF emailed to editor@ojepn.com

1. Editor acknowledges receipt, via email. Assigns manuscript number. Records submission date.

1. Editor aims to return Stage 1 decision within one week. Notifies authors of decision

1. If Stage 1 is conditional acceptance, Editor assigns reviewer(s) for full review. Aim for two
reviewers.

1. Reviewers aim to return full review to Editor within one month.

1. No later than one month, Editor returns such reviews as received to author, with supporting letter indicating needed actions.

1. Author returns modified manuscript, Editor decides whether to accept on own reading, or pass back to reviewers for further comment. 

1. Once accepted, author invited to send source files in appropriate format, and invoiced for payment if necessary. Editor requests Crossref DOI.

1. Author told production options are to either provide latex format that produces publication-ready PDF (no further proof reading or formatting provided by journal), or to pay for production of same (currently 100 GBP). 

1. Once formatted and paid, Editor creates landing page on ojepn.com, and adds paper to list of articles page on ojepn.com. Landing page URL used to update crossref entry.

1. Once crossref link is working, author notified of publication of paper.

## Post-acceptance production

1. If necessary, paper converted into latex format.

1. Latex format proof read for spelling, formatting, references. 

1. Latex source files uploaded to github repo using last part of DOI (2020-xxxx) as identifier.

1. PDF uploaded to ojepn.com. Landing page created. List of articles updated.

1. Crossref entry finalized

## Converting ODT to latex

1. Start with template.tex (Note: this needs updating from a recent article)

1. Convert ODT to TEX using pandoc (Linux command line: `pandoc ms.odt -o ms.tex`)

1. Insert  title, authors, affilitations, short title, header, DOI, abstract, keywords into .tex file

1. Copy and paste introduction

1. If equations, reformat these using `\begin{equation}` for numbered equations and `$` math mode for in-text equations. The template does not support unicode, so use math mode for Greek symbols etc. Any vaguely complex equation will probably need to be recoded from scratch.

1. Headings tend to be a bit screwed by pandoc, add manually.

1. Ideally, authors should have provided figures as separate PDFs. If they haven't, you can export them from the ODT file (right click in LibreOffice Writer, "Edit with External Tool"), although the resolution will suffer a bit.

1. Don't attempt to use bibtex for references. Instead, just cut and paste the references from the converted ODT, removing all the `\begin{quote}` and `\end{quote}` lines.



