# Formatting and other stylistic guidelines

## Use of English

- You may use US English, or UK English, but please pick one and stick to it. Either way, please note the following conventions:

	- 'which' should be preceded by a comma, 'that' should not.

	-  If the answer is 'him', use 'whom'. If the answer is 'he', use 'who'.

- Don't change tense arbitrarily. 

- Minimise the usage of quotation marks (for things other than quotations), italics, boldface, and so on, in your writing.

### Some examples of UK English

- 'whilst' can be used interchangeablely for 'while', where it is a conjunction or adverb.

### Some examples of US English

- US: 'labeled', 'modeled' ; UK: 'labelled', 'modelled'

## Titles and headings

- The article title should only capitalize the first word, proper nouns, and the first word after the colon (if you have a sub-title).

## Analysis

### Power calculations

- Power calculations should be performed a priori, i.e. to justify your choice of sample size on the basis of information available to you _before_ you collected the current dataset. Thus, power calculations should appear in your Method section; normally in the Participants subsection.

### Inferential tests

- Please consider using Bayesian analysis. If reporting a Bayesian analysis, please do not also report NHST for the same test - it's redundant and wastes space.

- Where concluding from a null, you must report either a Bayesian analysis, or some other recognised technique that provides evidence that a null has been found. Standard tests (e.g. t-tests, ANOVAs, etc) do not, on their own, provide this.

- When reporting any statistical method where there would have been more than one substantively different way to do it, report how you did it. For example, if calculating a Bayes Factor, what was your prior? Which software package did you use?

- For NHST, consider reporting your alpha value at the beginning of your results. If you do this, do not then report the individual p-values, which are largely meaningless beyond which side of your alpha level they appear.

## Figures

- The text on figures should not be noticeably smaller than the text in the body of the manuscript.

- Don't produce figures that are mainly empty space (whatever colour that space is). It makes the main subject of the figure unnecessarily hard to see.

## Citations 

- To include text before or after a reference, use this format:

	`\cite[before][]{Medin1988}`

	`\cite[after]{Medin1988}`

	`\cite[before][and after]{Medin1988}`

## References

- When citing software, include the version number in the note field of your bib file e.g
`note = {Version 0.4.2}`

- In your .bib file:

    - Every reference must have a DOI, unless no DOI for that reference exists.
	
	- Make sure the capitalization of fields (e.g. title, journal) is consistent with APA styling. You may need to used double-braces to achieve this in some cases e.g. `booktitle={{Handbook of Categorization in Cognitive Science}}`
	
	- You must format your DOI entry like this:
	
	`note = {\url{https://doi.org/10.46221/ojepn.2020.aa}}`
	
	In other words, use the `note` field, not e.g. a `doi` field. Include `\url`. Include `https://doi.org/` before the DOI code istelf. 

	- DO separate initials of authors, i.e. `J. K. Kruschke` rather than `J.K. Kruschke`. The latter results in only the first initial being displayed in the reference section.

	- DO NOT include 'a' etc. suffixes in the year, bibtex adds these for you. So, `year = {1996}` not `year = {1996a}`

	- DO NOT include a reference unless you cite it (it's harder for us to locate and fix format errors if there are a lot of uncited references).
	
	- For the same reason, DO NOT include fields that are not used by the journal (e.g. abstract, keywords).
	
	- If the article is in a journal, and the journal has an issue number, include the issue number.
