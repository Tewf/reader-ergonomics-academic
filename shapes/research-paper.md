# Shape: research paper

The shape of an empirical research article: IMRaD with a [structured abstract](../evidence/academic-papers/frame.md), the baseline named in [baseline](../evidence/academic-papers/baseline.md), plus the few additions that have evidence elsewhere.

## When to use it

- An empirical study (experiment, observational study, computational evaluation) reported to a journal, a conference or a preprint server.
- Not for a proof-centred mathematical article: a companion shape covers that.
- Not for a review, an essay or a humanities article, whose structure follows the argument rather than the study.
- Inside a publisher class (elsarticle, llncs, IEEEtran, acmart), keep the class for layout and metadata and take the section order from here; the class does not supply one.

## How each part maps to the evidence

| Part | What it does | Evidence | Grade |
|---|---|---|---|
| Title | states the finding or the question, since it is read first | Keshav 2007 | convention, untested |
| Structured abstract | Background, Methods, Results with numbers, Conclusions | Taddio 1994, Budgen 2008, Hartley 2004a | measured (information content) |
| Highlights, graphical abstract | optional extras some journals require | Elsevier highlights, Oska 2020 | convention, untested (attention only) |
| Introduction | territory, niche, this paper, then contributions and a map of the sections | Swales 1990, Hill 1982 | supported with caveat (describes practice) |
| Methods: plan and deviations | if the study was preregistered, the protocol and each departure from it with its reason; if not, that it is exploratory | Chambers 2013, Kerr 1998, Scheel 2021 | measured (for the format) |
| Methods: design, measures, analysis | enough detail to repeat the study, item by item | Turner 2012 | measured (completeness) |
| Results | one subsection per claim, a headline sentence first, a figure whose caption stands alone | Hubbard 2017, Keshav 2007 | supported with caveat |
| Discussion | the principal finding first, then comparison, limitations, implications | Hill 1982, Boutron 2010 | supported with caveat |
| Data and code availability | where the data, code and environment are, so the results can be re-run | Buckheit 1995, Pimentel 2019; the audits of availability statements (Gabelica 2022, Danchev 2021, Hamilton 2023) find "on request" weak, so give an archive and a version | supported with caveat |
| Reporting checklist | names the EQUATOR guideline followed, if one exists for the design; at computing venues, the venue's own checklist (NeurIPS, ACL) | Turner 2012, NeurIPS 2026, ACL 2023 | measured for EQUATOR (completeness); venue checklists convention, untested |
| Language-model use declaration | says whether and how a language model was used, worded to the venue's rule | ICMJE 2023, Nature 2023, ACL 2023, ICML 2023, NeurIPS 2025 | convention, untested |
| Declarations, references, appendix | funding, conflicts, contributions; the venue's reference style | ICMJE 2026 | convention, untested |

Each key (Author Year) is listed in [references](../evidence/bibliography.md).
No part of this shape has been tested against IMRaD on reader outcomes; [position](../evidence/academic-papers/position.md) says what would test it.

## The principles it applies

| Part | Principle |
|---|---|
| Title that states the finding; structured abstract | [overview first](https://github.com/Tewf/reader-ergonomics/blob/v1.0.0/principles/document/overview-first.md) |
| Contributions and a map of the sections, closing the introduction | [overview first](https://github.com/Tewf/reader-ergonomics/blob/v1.0.0/principles/document/overview-first.md), [signal the structure](https://github.com/Tewf/reader-ergonomics/blob/v1.0.0/principles/page/signal-the-structure.md) |
| Terms and measures defined in Methods before Results use them | [define before use](https://github.com/Tewf/reader-ergonomics/blob/v1.0.0/principles/document/define-before-use.md) |
| Results: one subsection per claim, its headline sentence first | [signal the structure](https://github.com/Tewf/reader-ergonomics/blob/v1.0.0/principles/page/signal-the-structure.md), [given before new](https://github.com/Tewf/reader-ergonomics/blob/v1.0.0/principles/sentence/given-before-new.md) |
| A figure whose caption stands alone, placed with the text that cites it | [draw relations](https://github.com/Tewf/reader-ergonomics/blob/v1.0.0/principles/page/draw-relations.md), [figure next to its text](https://github.com/Tewf/reader-ergonomics/blob/v1.0.0/principles/page/figure-next-to-its-text.md) |
| Headings on at most three levels | [shallow outline](https://github.com/Tewf/reader-ergonomics/blob/v1.0.0/principles/document/shallow-outline.md) |

## Skeleton

Copy this into a new file, or start from the LaTeX version, [research-paper.tex](research-paper.tex).

````markdown
# Title that states the main finding

First Author (affiliation, contact), Second Author (affiliation)

## Abstract

**Background.** The problem and the gap, in one or two sentences.

**Methods.** Design, sample and main measure.

**Results.** The main result with its number and interval.

**Conclusions.** What the result means, and its main limit.

**Keywords:** three to six terms a searcher would type.

## Highlights (optional)

> Three to five bullets of at most 85 characters each, only if the venue asks for them.

## 1. Introduction

> Establish the territory, show the gap, say what this paper does, list its contributions, and give a one-line map of the sections.

## 2. Methods

### 2.1 Plan and deviations

> If the study was preregistered, link the protocol and list every departure from it with its reason; if not, say that it is exploratory.

### 2.2 Design and materials

> Who or what was studied, how it was chosen, and with what, in enough detail to repeat it.

### 2.3 Measures and analysis

> Each outcome, how it was measured, and the analysis planned for it.

## 3. Results

### 3.1 First claim

> Open with the headline sentence of the result, then the number and its interval, then the figure.

Figure 1. A caption that says what the figure shows and what to conclude, readable without the text.

### 3.2 Second claim

> One subsection per claim, in the order of the contribution list.

## 4. Discussion

### 4.1 Principal finding

> The main result restated in one paragraph, without new data.

### 4.2 Comparison with prior work

> Where the result agrees or disagrees with earlier studies, and why.

### 4.3 Limitations

> What the design cannot show, and how large each threat is.

### 4.4 Implications

> What follows for practice or for the next study, kept within what the data support.

## 5. Conclusion

> Two or three sentences a reader could quote; no claim absent from the results.

## Data and code availability

> Where the data, code and computing environment are, under which licence, and how to re-run the analysis.

## Reporting checklist

> Name the reporting guideline followed (for example CONSORT or PRISMA) and attach the completed checklist.

## Declarations

> Funding, conflicts of interest, author contributions, acknowledgements.

## References

> In the venue's style; every entry with a DOI, an arXiv id or a stable URL.

## Appendix A. Supplementary material

> Material a specialist needs and a general reader can skip.
````
