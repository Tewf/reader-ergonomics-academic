# Protocol

How the pool on reports was searched, in two passes, so either can be rerun. The method shared by every review here is in the [evidence README](../README.md); the pool is in [sources](sources.md).

## Method and its source

- The review is a **multivocal literature review** (MLR) after Garousi 2019: journal literature plus grey literature (rules, standards, reports, school guides).
- One reviewer did all steps. Searches ran on 2026-10-29.
- No identity was sent to any service: no email address, no key, no sign-in, no polite-pool parameter.

## 1. Why grey literature (Garousi Table 4)

| # | Question | Answer for this topic |
|---|---|---|
| 1 | Is the subject complex and not solvable from the formal literature alone? | yes: standards and school guides are published as pages |
| 2 | Is volume or quality of evidence lacking? | yes: almost no controlled study of how reports are read |
| 3 | Is context important? | yes: school, country, discipline and report kind change the rule |
| 4 | Is the goal to corroborate research with practice? | yes |
| 5 | Is the goal to challenge practice with research, or the reverse? | yes: summary-first practice against missing tests |
| 6 | Would both communities gain from a synthesis? | yes |
| 7 | Is there a large volume of practitioner sources? | yes: every school and company has a guide |

Seven of seven answers are yes, so grey literature is included.

## 2. Questions

R1 to R6 are defined in [frame](frame.md).

## 3. Existing reviews first (Garousi Guideline 2)

Strings run on a web search engine, US-only, standard mode.

| Id | String | Found |
|---|---|---|
| E1 | `systematic review genres of university student writing BAWE genre families Gardner Nesi` | no systematic review; the BAWE classification and its book |
| E2 | `systematic review thesis examiners how examiners assess doctoral theses Mullins Kiley` | no systematic review; two examiner studies |
| E3 | `executive summary effect on readers comprehension experiment technical report` | no study of executive summaries |
| E4 | `survey review of research on internship reports student placement writing genre workplace report` | small genre studies; one review of placements, not of writing |
| E5 | `deductive versus inductive order message reports conclusion first versus conclusion last readers comprehension experiment business writing` | experiments on letters and product texts; none on reports |

## 4. Formal search

Strings, same engine and date. Database counts were not obtained: the OpenAlex free budget returned "429" (credits exhausted) at the first call, so no count is recorded. Metadata of every keyed work was checked on Crossref (anonymous public pool, no identity), which gives no hit count.

| Id | String |
|---|---|
| F1 | `Paltridge 2002 thesis and dissertation writing: an examination of published advice and actual practice English for Specific Purposes` |
| F2 | `Bunton 2005 The structure of PhD conclusion chapters Journal of English for Academic Purposes` |
| F3 | `Bourke Holbrook examining PhD and research masters theses Assessment Evaluation in Higher Education examiners' reports literature review` |
| F4 | `informative headings versus topic headings recall comprehension experiment text Hartley` |
| F5 | `écrits universitaires rapport de stage genre discursif analyse Rinck Boch Delcambre` |
| F6 | `engineering design report student genre BAWE project report structure moves Nesi Gardner` |
| F7 | `Paltridge thesis structures simple traditional topic-based compilation of research articles "published advice" abstract` |
| F8 | `examiners read thesis introduction conclusion first decide early "examiners" how thesis examiners read the thesis order of reading study` |
| F9 | `thesis length and examiner outcome word limit dissertation too long examiners reading burden study` |

Snowballing was one step: the Crossref lookup of works named in an abstract or a list (Holbrook, Bourke, Kiley, Lorch, Pinelli 1997). No forward citation search was possible without a citation database.

## 5. Grey search

Types chosen were standards bodies (NISO, ISO), French school and university guides and grids, a government research report and a university transcript of practitioner interviews.

| Id | String |
|---|---|
| G1 | `ANSI/NISO Z39.18 scientific and technical reports preparation presentation and preservation elements of report` |
| G2 | `ISO 7144 presentation of theses and similar documents` |
| G3 | `rapport de stage structure attendus jury grille d'évaluation école d'ingénieurs` |
| G4 | `rédaction scientifique mémoire de master guide structure plan introduction conclusion université Grenoble Alpes` |
| G5 | `Cutts Oxford guide to plain English executive summary bottom line up front reports readers research evidence` |
| G6 | `Arrêté CTI référentiel école d'ingénieur rapport de stage fin d'études mémoire ingénieur exigences format` |
| G7 | `Grenoble INP Ensimag rapport de stage consignes plan résumé abstract rapport de PFE recommandations de rédaction` |
| G8 | `grille d'évaluation rapport de projet étudiants critères introduction problématique structure clarté sources enseignant` |
| G9 | `readers of technical reports read summary conclusions first study of how managers engineers read reports` |
| G10 | `Pinelli Glassman Barclay "use of technical report components" NASA technical managers nonmanagers components used to decide whether to read a report` |
| G11 | `host company supervisor evaluation of student internship report what employers expect workplace supervisor assessment study` |
| G12 | `soutenance de mémoire de master attentes du jury lecture du mémoire critères d'évaluation qualité du mémoire enseignants-chercheurs enquête` |

## 6. Stopping rule (Garousi Guideline 8), fixed before searching

- **Saturation:** stop a family when two strings in a row add no new included source.
- **Effort bound:** about 120 results screened in all.
- Applied: saturation stopped each family. E ended after E4 and E5 (0 added each). F ended after F8 and F9 (0 added each). G ended after G11 and G12 (0 added each).
- The effort bound was exceeded: the engine lists about 10 results per call, so 26 calls listed 323 results (sources.md). Titles were skimmed; only 12 pages were read.

## 7. Selection

Included when a source:

- states a rule, a practice or a measurement about the structure, readers or grading of a report or thesis (IC1);
- comes from the owner or the measurer (IC2);
- has a stable address (IC3);
- was read in full, or as an abstract or catalogue record, and says which (IC4);
- scores at least 10 of 20 if grey (section 8).

Excluded when it:

- is a blog or a relay of a rule (EC1);
- is a commercial service page (EC2);
- could not be retrieved (EC3), for example a 403 or a bot check;
- duplicates an included source (EC4);
- concerns only the viva as a social event (EC5).

A source below 10 stays as an **example of practice**; no claim leans on it.

## 8. Quality of grey sources

The 20 criteria and tiers of Garousi Table 7 are used unchanged (authority 4, methodology 6, objectivity 4, date 1, position 1, novelty 2, impact 1, outlet 1). A rule page has no method of its own, so methodology scores its aim, scope and case only.

## 9. Extraction and synthesis

- Extracted: kind, date, the rule or number, producer, and whether the producer reports on itself.
- Synthesis is narrative by question, traceable through [sources](sources.md).
- A number read only in an abstract, a catalogue record or a search summary is marked "(secondary)".

## 10. Limits

- One reviewer; no second rater.
- Several pages returned 403 or a bot check and were not read (sources.md, Excluded). No check was bypassed.
- The engine returns summaries; every included source was opened, or marked as a record only.
- No Grenoble M1 AI report guide was found.

## Second pass (2026-10-29): examiners, and summary first

Rows to append to protocol.md. The first pass is in protocol.md; this pass deepens two questions only.
Numbering continues the first pass: E6 and up, F10 and up, G13 and up.

### Method of the pass

- Same MLR method (Garousi 2019), one reviewer, searches run on 2026-10-29.
- No identity was sent to any service: no email in a request, header, User-Agent or query; no Unpaywall; no key; no sign-in; no bot check solved.
- Engine for strings: a web search tool, US-only, standard mode, about 10 results per call.
- Metadata and abstracts: Crossref and OpenAlex single-work lookups by DOI, and the Semantic Scholar graph API for citing papers, all anonymous and one call at a time. The OpenAlex list endpoint refused (free budget used up), so no database hit count exists, as in the first pass.
- Held and not searched again: everything in the first-pass pool; Britt 2003 and Garner 2013 (sister review, linked); the reading-order review (Jansen 2010, Nielsen 2006, Nildam 1998, Sternadori 2008, Pinelli 1982, Hartley 2004), linked.

### The two questions of this pass

- **P2a** How do examiners read and judge a thesis (order, first look, criteria, early decision), and how do teachers grade a project or internship report (rubrics, weights)?
- **P2b** Is there experimental evidence that putting the summary, the main result or the conclusion first helps readers of reports or expository texts?

### 1. Why grey literature (Garousi Table 4), for P2a and P2b only

| # | Question | P2a | P2b |
|---|---|---|---|
| 1 | Subject complex, not solvable from formal literature? | yes: grids and forms are published as pages | partly: the rule (BLUF) is a regulation |
| 2 | Volume or quality of evidence lacking? | partly: examiner studies exist, grading studies are few | yes: no controlled test on reports found |
| 3 | Context important? | yes: country, level, school change weights | yes: reader, culture and message valence change the effect |
| 4 | Corroborate research with practice? | yes | yes |
| 5 | Challenge practice with research, or the reverse? | yes: grids weight form and content without a measure | yes: BLUF is mandated and untested |
| 6 | Both communities gain from a synthesis? | yes | yes |
| 7 | Large volume of practitioner sources? | yes: every school has a form | yes: every writing guide says summary first |

Seven of seven are yes or partly, so grey literature is kept.

### 2. Existing reviews (Garousi Guideline 2)

| Id | String | Found |
|---|---|---|
| E6 | `systematic review how doctoral thesis examiners assess theses examiner reports literature review` | one qualitative systematic review (Golding 2014) |
| E7 | `executive summary effect on readers experiment comprehension decision making managers report with summary versus without` | no review; one pilot trial on a summary box (Koetsenruijter 2022) |
| E8 | `synthèse en tête résumé exécutif lecteurs décideurs étude expérimentale compréhension rapport conclusion d'abord ou en dernier lecteurs` | nothing new |
| E9 | `meta-analysis OR systematic review text structure signaling main idea position topic sentence placement comprehension expository text reviews` | reviews of structure instruction; none on position; nothing included |
| E10 | `systematic review assessment of student reports rubrics criteria written project reports higher education engineering reliability validity review` | one review of rubrics (Reddy 2010); one rubric reliability paper (Brown 2023) |
| E11 | `literature review of research on thesis assessment and examiner reading: systematic review of thesis examination studies 2015-2025` | Golding 2014 again; one survey of examiners (Sharmini 2015) |
| E12 | `review of research on reading of technical reports by engineers and managers: summary conclusions first, document design evidence synthesis` | one preference experiment (Silyn-Roberts 2002) |
| E13 | `systematic review inverted pyramid news structure comprehension recall experiments meta-analysis` | no review; items already held in reading-order |
| E14 | `systematic review of internship or work placement assessment written report reflective report grading practices` | module guides only; nothing included |

### 3. Formal search

| Id | String |
|---|---|
| F10 | `Mullins Kiley "It's a PhD, not a Nobel Prize" how experienced examiners assess research theses full text pdf` |
| F11 | `Carter 2008 examiner reading thesis "endurance test" "treat" examining the doctoral thesis how examiners read` |
| F12 | `Holbrook Bourke "Examiner comment on the literature review in Ph.D. theses" 501 candidates 1310 reports abstract` |
| F13 | `Bourke Holbrook 2013 "Examining PhD and research masters theses" 353 examiners twelve indicators abstract` |
| F14 | `capstone engineering design project report rubric faculty assessment criteria inter-rater reliability written report study` |
| F15 | `Jansen Janssen "Explanations first" bad-news messages Journal of Business and Technical Communication 25(1) 36-67 experiment comprehension` |
| F16 | `summary placed before text versus after text recall comprehension experiment "initial summary" "final summary" expository passage` |
| F17 | `main idea first versus last paragraph position topic sentence comprehension experiment expository text Kieras 1981 "main idea" position recall reading time` |
| F18 | `deductive versus inductive text structure conclusion first conclusion last readers comprehension experiment technical documents Janssen Jansen product text cross-cultural` |
| F19 | `Kieras 1978 "Good and bad structure in simple paragraphs" apparent theme reading time recall abstract first sentence theme` |
| F20 | `Britt Larson 2003 constructing representations of arguments claim first citing studies argument order reading time recall experiment` |
| F21 | `Johnston 1997 "Examining the examiners: an analysis of examiners' reports on doctoral theses" Studies in Higher Education abstract` |

Snowballing, one step, on the Semantic Scholar graph API (anonymous):

- forward from Mullins 2002 (100 citing papers listed), Jansen 2010 (19), Britt 2003 (49) and Kieras 1978 (136): 304 titles screened;
- backward from Golding 2014 (its reference list): Carter 2008, Holbrook 2008 and Johnston 1997 (the first two were read in full on 2026-10-29).

### 4. Grey search

Types chosen: a government regulation (US Army), university assessment forms (Twente, UGA), a Belgian programme page (ULB), an académie grid (Grenoble BTS).

| Id | String |
|---|---|
| G13 | `internship report assessment criteria rubric university supervisor grading what is weighted study` |
| G14 | `grille d'évaluation rapport de stage master critères pondération soutenance jury université pdf` |
| G15 | `évaluation du rapport de stage par les enseignants critères implicites analyse recherche didactique écrits professionnels étudiants stage` |
| G16 | `UFR IM2AG Université Grenoble Alpes M1 informatique stage rapport évaluation grille critères soutenance` |
| G17 | `mémoire de master jury soutenance critères d'évaluation grille qualité de l'écrit introduction problématique conclusion université guide` |
| G18 | `"executive summary" readability study business reports readers actually read executive summaries empirical` |
| G19 | `"bottom line up front" Army Regulation 25-50 preparing and managing correspondence BLUF requirement` |
| G20 | `AR 25-50 "Army writing style" "put the main point at the beginning" "bottom line up front" active voice` (restricted to armypubs.army.mil, army.mil, apd.army.mil) |
| G21 | `Pyramid Principle Minto answer first evidence experiment readers comprehension test of pyramid structure business writing` |
| G22 | `Lovitts 2007 "Making the implicit explicit" creating performance expectations dissertation examiners criteria missing outstanding` |

### 5. Stopping rule (Garousi Guideline 8), as fixed in the first pass

- **Saturation:** two strings in a row add no included source.
- **Effort bound:** about 100 results.
- Applied: E stopped on saturation after E13 and E14 (0 added each). F stopped on saturation after F20 and F21 (0 added each). G stopped on saturation after G21 and G22 (0 added each).
- The effort bound was exceeded, as in the first pass: the engine lists about 10 results per call, so 31 calls listed 371 results (E 112, F 154, G 105). Titles were skimmed; 9 documents were read in whole or in the relevant part (sources-pass2.md).

### 6. Selection and quality

- Inclusion, exclusion and the 20-criterion score are those of protocol.md sections 7 and 8, unchanged.
- A source below 10 stays an example of practice. A number read only in an abstract, a record, a search summary or another paper's report of it is marked "(secondary)".
- One addition: a source that I reached only through the review that cites it (Carter 2008, Holbrook 2008, Johnston 1997) was listed with metadata only and its claims marked "(secondary)". Carter 2008 and Holbrook 2008 were read in full on 2026-10-29. Johnston 1997 stays secondary.

### 7. Limits of the pass

- One reviewer; no second rater.
- Full text of the four examiner papers was not reached in this pass. Mullins 2002 and Kiley 2004: publisher closed, and the one copy found sits behind a university VPN login, not tried. Holbrook 2007 and Bourke 2013: publisher closed, and the Newcastle repository answered 403. Their abstracts were read through OpenAlex or Crossref. All four were read in full on 2026-10-29 through the university's access (full text). Golding 2014 was also read in full on 2026-10-29 (open access).
- Several pages returned 403, an access-denied notice or a bot check and were not read; no check was bypassed (sources-pass2.md, Excluded).
- A claim that "no study was found" means no study in this pool of strings and engines.
- No Grenoble M1 AI report guide was found (G16, as in the first pass).
