# State of the art

An **upper bound** here is the best result achieved, by whom, measured how.
A **limit** is a result showing that a part does not deliver what it is assumed to deliver.
A **trend** is a description of practice, with no comparison of formats.

- **adoption**: a count of how many venues, papers or developers follow a practice;
- **lower bound**: an estimate that undercounts by construction;
- **open**: a question for which no study was located.

| Sub-question | Record holder | Method | Measure | Kind |
|---|---|---|---|---|
| How widespread is IMRaD in medicine? | Sollaci 2004 | 1,297 articles, 4 journals, 1935-1985 | above 80% in the 1970s, sole pattern in the 1980s | upper bound |
| How widespread elsewhere? | Lin 2012; Moskovitz 2024 | hand-coded corpora, 39 disciplines; STEM by study type | plain IMRD not the default; under half in engineering and social science | limit |
| Does a checklist raise completeness? | Turner 2012 | Cochrane review, 50 non-randomised evaluations, 16,604 trials | allocation concealment 45% vs 22% (RR 1.81, 99% CI 1.25 to 2.61) | upper bound |
| Is reporting then complete? | Turner 2012 | same | "remains sub-optimal" in endorsing journals too | limit |
| Does endorsement help for guidelines other than CONSORT? | Stevens 2014 | systematic review, 101 guidelines, 26 evaluations of nine of them | PRISMA summed score only (SMD 0.53, 99% CI 0.02 to 1.03, endorsing against non-endorsing journals); insufficient evidence for the rest | limit |
| Does a structured abstract hold more information? | Taddio 1994 | 300 abstracts before and after the switch, 33 criteria | quality 0.57 vs 0.74 | upper bound |
| Same, outside medicine | Budgen 2008 | randomised paired judgement, 64 judges | completeness +6.65 on an 18-item questionnaire, clarity +2.98 on 1-10 | upper bound |
| Does it speed up search? | Hartley 1996 | simplified abstracts | faster and more accurate, as summarised in Hartley 2004a | upper bound |
| Same, with real database abstracts | studies 15 and 17 in Hartley 2004a | timed search on MEDLINE abstracts | no speed advantage | limit |
| Does searching by labelled field help? | Booth 1997 | simulated database, ten searches | precision rose and recall fell; figures not verified | limit |
| Is it easier to read? | Hartley 1997 | eight studies: formulas, sentence reordering, reader ratings | formula scores higher only when authors rewrote the abstract; readers rated structured ones easier | limit |
| Is it more accurate? | Pitkin 1999; Hartley 2000 | abstract data checked against the body | 18% to 68% of medical abstracts deficient; no format difference in psychology | limit |
| Does a visual abstract draw attention? | Oska 2020 | crossover, 40 articles, three tweet forms in random order | mean views 1,351 vs 639 (citation) vs 732 (key figure) | upper bound |
| Does it improve understanding? | none found | none | no controlled comprehension study located | open |
| Does results-blind review change what is published? | Scheel 2021 | 71 Registered Reports vs 152 standard reports, first hypothesis | 44% vs 96% positive results | upper bound |
| Is the quality judged higher? | Soderberg 2021 | 353 reviewers, 29 Registered Reports vs 57 comparisons, 19 criteria | methodological rigour +0.99 on a -4 to +4 scale; novelty no difference | upper bound |
| Does a code-and-text bundle reproduce? | Pimentel 2019 | re-ran 863,878 Python GitHub notebooks with a valid execution order | 24.11% ran without error, 4.03% gave the same results | limit |
| How long does a reading last? | Tenopir 2008 | repeated surveys since 1977, last-reading incident | 48 minutes (1977) to 31 minutes (2005) | trend |
| Where do experienced readers look? | Hubbard 2017 | survey, 260 undergraduates and researchers in biological sciences at one UK university, section ranking | figures and results first, introduction last | trend |
| Is scientific prose getting harder? | Plavén-Sigray 2017 | 709,577 abstracts, FRE and NDC | FRE falls with year (r = -0.93) | trend |
| Is there evidence for plain-language summary criteria? | Stoll 2022 | systematic review, 90 articles, 33 empirical | evidence on criteria scarce | limit |

### Most adopted (a practice record)

| Sub-question | Record holder | Method | Measure | Kind |
|---|---|---|---|---|
| Is a reporting checklist required of every submission in ML? | NeurIPS (since 2019), ACL venues (since 2020) | venue rules | mandatory at submission; NeurIPS 2026 has 16 questions | adoption |
| How many papers come with code in ML? | Pineau 2021 | 2019 NeurIPS submissions | about 40% at submission, 74.4% at camera-ready | adoption |
| How many NLP submissions link code? | Magnusson 2023 | 10,405 checklist responses | 45.9% | adoption |
| How many models carry a card? | Liang 2024 | 74,970 Hugging Face repositories | 44.2% by one count in the preprint, 90.5% of downloads | adoption |
| Are artifacts common where evaluation exists? | Winter 2022 | decade of SE and PL conferences | about 90% of eligible 2020 PLDI articles | adoption |
| How many publishers give AI guidance? | Ganjavi 2024 | top 100 publishers and journals, 2023 | 24% and 87% | adoption |
| How many statements say "on request"? | Gabelica 2022 | 3,416 BMC statements | 42% | adoption |
| How transparent are industry AI developers? | Bommasani 2024 | 14 developers, 100 indicators | mean 58 of 100 | adoption |
| How many STM publishers have an author policy on AI chatbots? | Bhavsar 2025 | audit of 162 publishers, 2023-09 to 2023-12 | 56 (34.6%) | adoption |
| How many health journals instruct on plain-language summaries? | Gainey 2022 | scoping review of 534 journals | 27 | adoption |
| How many ML papers share code and data? | Coakley 2026 | 56,800 papers, five AI venues | 11% in 2014, 64% in 2024 (preprint) | adoption |
| How many AI start-ups publish? | Loisel 2026 | 317 firms, 1998-2025 | more than half (52.4%) have no qualifying output (preprint) | adoption |

### Best evidence (a research record)

| Sub-question | Record holder | Method | Measure | Kind |
|---|---|---|---|---|
| Does an ML checklist change reporting? | Magnusson 2023 | pre-checklist sample of 50 papers against self-reported answers | 8 of 10 items up | upper bound (confounded) |
| Are checklist answers accurate? | Pineau 2021 | reviewers checked code claims | 71.5% confirmed | limit |
| Did documentation improve before the checklists? | Coakley 2026 | same corpus, trend by year | gains predate the checklists; the authors infer an open-science norm | limit (preprint) |
| Does a prompt at a set editorial point raise compliance? | Evanko 2025 | before and after, one publisher | RRIDs in published articles 33% to 65%; code capsules 1.4% to 4.6% | upper bound (uncontrolled, owner's data) |
| Do artifact badges raise citations? | Winter 2022 | corpus, decade of AE | no significant gain | limit |
| Same, with correlation only | Heumüller 2020 | 789 ICSE papers | small positive correlation | upper bound (observational) |
| Does a badge raise sharing? | Kidwell 2016 | before and after with comparison journals | under 3% to 39% | upper bound |
| Does a data mandate raise sharing? | Hardwicke 2018 | interrupted time series | 25% to 78% | upper bound |
| Does a statement predict real availability? | Danchev 2021 | 487 trials, declared against actual | 68.6% declared, 0.6% public | limit |
| Does sharing on request work? | Stodden 2018 | 204 papers, request and re-run | 44% obtained, 26% reproduced | limit |
| Does a datasheet change what an engineer notices? | Boyd 2021 | think-aloud, 23 participants | more ethical issues, earlier | upper bound (small) |
| Does a model card raise use? | Liang 2024 | difference in differences, 42 models | +29.0% in one batch | upper bound (one batch) |
| Does a plain summary beat a text summary? | Buljan 2018 | three randomised trials | no knowledge difference | limit |
| Which summary type raises perceived understanding? | Bredbenner 2019 | randomised, 538 participants | video and plain language ahead | upper bound |
| Is a significance statement simpler? | Markowitz 2024 | 34,584 PNAS papers | d near 0.3 on word simplicity | trend |
| How much biomedical writing is LLM-processed? | Kobak 2025 | excess vocabulary, 15 million abstracts | at least 13.5% (2024) | lower bound |
| Same, by field and venue | Liang 2025 | mixture model, 950,965 papers | up to 17.5% in computer science | upper bound (estimate) |
| Does STAR Methods improve reporting? | none found | none | no study located | open |
| Do release blog posts or technical reports change reading or citing? | none found | none | no study located | open |
| Does authors' declared AI use match estimated use? | none found | none | no study located | open |
| Do reviewers follow an AI rule? | Kim 2026 | randomised policy and survey, N = 1,486 reviewers and chairs | 22.5% under a ban said they used an LLM (self-report, preprint) | limit |

## Reading the table

- Every record concerns an abstract, a checklist, a review format or a bundle; none compares a whole article written in two shapes.
- Any claim that IMRaD helps readers of full articles is therefore graded convention, untested (position.md).
- The trends describe readers and prose; they do not say which shape serves those readers best.
- The upper bounds for compliance come from a venue or publisher measuring itself (Evanko 2025, ICML 2026b); an outside measurement of the same is rare.
