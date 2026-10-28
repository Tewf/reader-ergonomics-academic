# Protocol

This file records how the pool of sources for this topic was built, so that the search can be repeated.

It follows Garousi 2019 for a multivocal literature review (MLR, defined in the [evidence README](../README.md)) in a lighter form.

Garousi 2019 was written for software engineering. Its guidelines are applied here to presentations, a field with a large teaching and speaking practice beside its research. The formal pool predates the protocol, and this file says so.

## 1. Why grey literature (Garousi Table 4, seven questions)

| # | Question | Answer for presentations |
|---|---|---|
| 1 | Complex subject, not solvable by the formal literature alone | yes: speaker, room and format rules are mostly practice |
| 2 | Lack of volume, quality or consensus of evidence | yes: few live-talk studies, bundled factors |
| 3 | Context matters | yes: audience, length, room, field |
| 4 | Goal to check research against practical experience | yes |
| 5 | Goal to challenge practice rules with research | yes: 30 point, 10 minutes, 3 seconds |
| 6 | Synthesis useful to both communities | yes |
| 7 | Many practitioner sources | yes: every grey string returned speaker guides and workshops |

Seven of seven are yes, so grey literature is included.

## 2. Questions

- Q1 Does on-screen text that repeats the voice help or hurt, and which principles apply to a paced medium?
- Q2 Does showing slides help, and which slide design helps?
- Q3 What does the speaker add: gesture, face, enthusiasm?
- Q4 What makes slides legible and accessible in a room?
- Q5 How are talks built, and how do questions and discussion work?
- Q6 What does practice recommend and adopt, and how does it compare with Q1 to Q5?

## 3. Existing reviews (Guideline 2)

| Id | String, as run | Results screened | Included |
|---|---|---|---|
| E1 | systematic review meta-analysis PowerPoint slides student learning outcomes | 10 | 0 |
| E2 | meta-analysis multimedia learning principles review of reviews Mayer | 10 | 2 (Noetel 2022, Cromley 2025) |
| E3 | systematic review scientific conference presentations oral presentation slides effectiveness | 9 | 1 (Blome 2017) |
| E4 | meta-analysis instructor visibility lecture video learning outcomes 2022 2023 2024 | 10 | 3 (Polat 2022, Zhu 2024, Heidig 2024) |
| E5 | scoping review slide design PowerPoint lectures higher education text density images | 9 | 0 (Le Blanc 2025 came through G4) |
| E6 | meta-analysis teacher gestures learning students instruction | 9 | 0 |

Engine for E, F and G strings: a general web search tool (one engine, US-based, returns a summary and links), run on 2026-10-28.

## 4. Formal search

- The formal pool was built by a narrative search plus snowballing (frame.md lists the terms), not by screening database counts. The counts below only describe the terms.
- Query form: `https://api.openalex.org/works?filter=title_and_abstract.search:<terms>&per_page=1`, field `meta.count`, run 2026-10-28.
- These ten were run with the words unquoted, so each count is "all words anywhere in title or abstract", not a phrase. The count for assertion-evidence is mostly noise from the two common words.

| Terms | Count |
|---|---|
| multimedia learning principles | 4474 |
| cognitive theory of multimedia learning | 3223 |
| cognitive load theory | 12466 |
| redundancy effect | 17159 |
| assertion-evidence | 20927 |
| instructor presence | 5778 |
| gesture comprehension meta-analysis | 27 |
| conference presentation genre | 824 |
| conference presentation | 160781 |
| discussion sessions | 68325 |

- Not run: the other terms of frame.md (PowerPoint, slide design, pedagogical agent, split attention, modality, segmenting, the acronyms and the author names). The service answered HTTP 429 after these ten, with a retry delay of about five hours.
- Snowballing: forward from Garner 2013 (41 citing records when listed in an earlier session; 4 kept: Wolfe 2023, Wolfe 2025, Alzayed 2023, Sripradith 2023). In this round, backward from Bramble 2026 (strings F1, F2 below): 2 kept (Alley 2007, Root Kustritz 2014).

| Id | String, as run | Screened | Included |
|---|---|---|---|
| F1 | Diesel assertion-evidence geoscience lecture slides test scores study | 10 | 2 (Alley 2007, Root Kustritz 2014) |
| F2 | Wolfe assertion-evidence slides computer science course exam scores study | 9 | 0 (no computer science exam study found) |

## 5. Grey search

Types and producers, with the reason for each (Guideline 6):

| Type | Producers | Why |
|---|---|---|
| Speaker guidance | TED and TEDx | the largest talk programme |
| Conference and society speaker guides | scientific societies, ACM events, USENIX | the rules authors of papers receive |
| Accessibility guides | ACM SIGACCESS, ACM events | access to a paced medium |
| University teaching centres | UNB, others | rules for lecturers |
| Practitioner books and sites | Duarte, Reynolds, Leonhard Center | the most read design advice |
| Formats | PechaKucha, Ignite, Lessig method | pace fixed by rule |
| Company practice | Amazon memos | replacing slides |

Strings, N = 10 results screened per string (title and the engine's summary); pages opened in full are counted apart.

| Id | String, as run | Screened | Opened | New included |
|---|---|---|---|---|
| G1 | TEDx speaker guide slides presentation tips | 9 | 1 | 0 (TED 2026 re-found) |
| G2 | scientific conference oral presentation guidelines for speakers slides society | 10 | 1 | 1 (SSP 2026); IEEE guide not read, certificate error |
| G3 | accessible presentation guidelines slides conference speakers | 10 | 1 | 1 (ACM 2026) |
| G4 | teaching center lecture slides design principles evidence-based | 10 | 2 | 2 (Bramble 2026, Le Blanc 2025) |
| G5 | assertion-evidence slide design workshop guide scientists | 10 | 1 | 0 (Leonhard Center 2026 re-found) |
| G6 | Amazon six-page narrative memo meetings instead of PowerPoint study hall | 10 | 0 | 0 (Bezos 2018 re-found) |
| G7 | how to give a good talk slides advice computer science researchers guide | 10 | 0 | 0 |
| G8 | PechaKucha Ignite 20 slides format presentation learning effectiveness study | 10 | 3 | 3 formal (Liao 2020, Warmuth 2021, Bakcek 2020) |
| G9 | Rector accessible presentation guide SIGACCESS slides speakers | 10 | 1 | 1 (Rector 2019) |
| G10 | Lessig method presentation style one word per slide origin Takahashi | 10 | 0 | 0 |
| G11 | ACM SIGPLAN OR USENIX OR NeurIPS conference talk instructions for speakers slides guidance | 40 | 0 | 0 |
| G12 | Garr Reynolds Presentation Zen design principles restraint simplicity naturalness slides | 10 | 0 | 0 |

- Totals for G1 to G12: 149 results screened, 10 pages or abstracts opened in full, 8 new sources (4 grey, 4 formal). Duarte 2026 was also opened, for scoring only. E1 to E6 screened 57 results and F1, F2 19; the E and F strings added 8 formal sources.
- Excluded without opening, by type: coach and template-vendor blogs (tier 3, repeating TED or Duarte); event listings and logistics pages; satire and course notes without authority; the same page found twice.
- Seen, not retrieved: two IEEE conference guides (TLS certificate could not be verified; no workaround attempted).

## 6. Stopping rule (stated before the search)

- **Effort bounded:** the top 10 results of each string (N = 10).
- **Saturation:** stop after 3 consecutive strings that add no new concept (k = 3).
- Applied: G10, G11 and G12 added no new concept (concepts: numeric size or text limits, sentence headlines, no slides, pacing, accessibility, handouts, Q&A, timing), so the search stopped after G12.
- New concepts by string:
  - G2: limits on title and line length.
  - G3: speak slide text aloud, describe visuals.
  - G4: note-taking handouts.
  - G8: outcome studies of fixed pacing.
  - G9: share slides a week ahead, avoid animation.

## 7. Selection

- Include: a source that states a rule or gives evidence on Q1 to Q6, in English, a talk or lecture with slides as its unit.
- Exclude: sources about posters, online meetings or video production; pages that repeat another page; sources unreadable here.
- A grey source is scored (section 8); one under 10 is kept only as an example of practice.

## 8. Quality of grey sources (Guideline 11, Table 7)

- 20 criteria, each 1, 0.5 or 0: authority of the producer (4), methodology (6), objectivity (4), date (1), position among related sources (1), novelty (2), impact (1), outlet type (1).
- Impact is read here as 1 when a count or derived guides were seen, 0.5 for evident wide use or an owner's claim, 0 otherwise.
- Outlet is 1 for books, standards and reports, 0.5 for owner guides and annual reports, 0 for blogs.
- Books known from a catalogue page only are scored on what that page shows; sources.md says so.
- Threshold 10 of 20 (Garousi): 12 of 24 grey sources are under it.

## 9. Extraction and synthesis

- Per source: producer, date, claim, number, evidence cited, limits.
- Synthesis is narrative by question; each claim traces to a row of sources.md.

## 10. Limits

- One reviewer; no inter-rater agreement; scores are judgements.
- One search engine that personalises and changes; results of 2026-10-28 may not repeat.
- Screening used titles and engine summaries; secondary numbers are marked "(secondary)".
- Formal side: ten of the frame terms counted, the pool not screened from them.
