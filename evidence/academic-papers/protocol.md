# Protocol

This file records how the pool of sources was built. With it the search can be repeated; the pool itself is in [sources](sources.md).

## Method and its source

- The review is a lighter **multivocal literature review** (MLR): journal literature plus **grey literature**, meaning sources outside peer-reviewed journals, proceedings and scholarly monographs: rules, reports, pages, practitioner books.
- Formal here means peer-reviewed articles, scholarly monographs and researchers' preprints with a method; trade and practitioner books count as grey tier 1.
- The guideline is Garousi 2019, summarised in the [method](../README.md#method). It was written for software engineering; its steps are applied here to publication science, and its quality list is used unchanged.
- "Lighter" means the formal search was not rerun from scratch (section 4), and the grey search was run with stated strings (section 5).
- One reviewer did all steps. Searches ran on 2026-10-28.

## 1. Why grey literature (Garousi Table 4)

| # | Question | Answer for this topic |
|---|---|---|
| 1 | Is the subject complex and not solvable from the formal literature alone? | yes: venues and publishers set the rules, and the rules are published as pages |
| 2 | Is volume or quality of evidence lacking? | yes: many rows are open (state-of-the-art.md) |
| 3 | Is context important? | yes: field and venue change the rule |
| 4 | Is the goal to corroborate research with practice? | yes |
| 5 | Is the goal to challenge practice with research? | yes: "on request" statements, highlights |
| 6 | Would both communities gain from a synthesis? | yes |
| 7 | Is there a large volume of practitioner sources? | yes: every publisher and venue |

Seven of seven answers are yes, so grey literature is included.

## 2. Review questions

| Id | Question | Strands |
|---|---|---|
| Q1 | How are articles ordered, and how common is each order? | 1, 3, 8 |
| Q2 | Which front-matter formats do publishers require, and what do they do for readers? | 4, 12 |
| Q3 | Do checklists and reporting guidelines change what is reported? | 2, 9 |
| Q4 | Do availability statements and badges match real availability? | 10, 13 |
| Q5 | What do venues require about language-model use, and how much use is estimated? | 15, 16 |
| Q6 | How do industry labs publish? | 14 |
| Q7 | How do researchers read? | 5, 6, 7 |

## 3. Existing reviews first (Garousi Guideline 2)

Eight strings and four named lookups, run on a web search tool; each result list was read for reviews, scoping reviews and audits.

| Id | String | Found |
|---|---|---|
| E1 | systematic review IMRaD structure of scientific articles | no review of IMRaD |
| E2 | systematic review effectiveness of reporting guidelines endorsement completeness of reporting meta-research | Stevens 2014 |
| E3 | systematic review graphical abstract visual abstract effect on dissemination and comprehension | Krukowski 2023 (narrative) |
| E4 | scoping review plain language summaries of research articles effectiveness | Stoll 2022, Gainey 2022 |
| E5 | systematic review structured abstracts readability information content | nothing beyond Hartley 2004a |
| E6 | machine learning reproducibility checklists survey review | Magnusson 2023 (held), Coakley 2026 |
| E7 | scoping review journal policies generative AI use authors disclosure | Bhavsar 2025 |
| E8 | systematic review of scientific writing guidance interventions | Galipeau 2015 |

- Named lookups after E2 and E8: Blanco 2019 (recalled from prior reading, then searched and checked), the Galipeau protocol, graphical-abstract reviews, the Bhavsar audit.
- Each review is placed in review.md strand 0 with how this review differs.

## 4. Formal search

The formal pool was built by a narrative search plus backward and forward snowballing, not by screening the counts below.
The counts only record how large each term's literature is.

- **Backward** from Sollaci 2004, Hartley 2004a, Turner 2012, Pineau 2021, Liang 2025.
- **Forward** from Sollaci 2004 (Lin 2012, Moskovitz 2024), Pineau 2021 (Magnusson 2023, Coakley 2026), Hartley 2004a (Hartley 2014).
- **Count method:** OpenAlex, `https://api.openalex.org/works?filter=title_and_abstract.search:"<term>"&per_page=1`, field `meta.count`, one run per term.
- **Status:** the free daily budget of the API was exhausted on 2026-10-28 (error "Rate limit exceeded"), so the 18 terms were
  counted on 2026-10-29 at 00:05 UTC, each as a quoted phrase.

| Term (frame.md) | OpenAlex count |
|---|---|
| IMRaD | 1 893 |
| create a research space | 213 |
| structured abstract | 3 524 |
| reporting guideline | 2 455 |
| scholarly reading | 410 |
| registered reports | 10 183 |
| executable paper | 58 |
| abstract readability | 52 |
| reproducibility checklist | 180 |
| artifact evaluation | 1 096 |
| model cards | 532 |
| plain language summary | 21 145 |
| data availability statement | 4 226 |
| foundation model transparency | 15 |
| excess vocabulary | 15 |
| generative AI policy | 119 |
| graphical abstract | 64 463 |
| datasheets for datasets | 65 |

## 5. Grey search

**Types chosen**, with the reason each is where rules and practice are written:

| Type | Producers | Why |
|---|---|---|
| Publisher author guides | Elsevier, Taylor & Francis, PLOS, Springer Nature | they fix front matter and AI rules |
| Venue calls, checklists, policies | NeurIPS, ICLR, ICML, ACL | they fix checklists and AI rules in ML |
| Standards and policy bodies | ICMJE, COPE, Center for Open Science, EQUATOR | they set cross-journal norms |
| Platform policies | arXiv, bioRxiv | they decide what is posted |
| Lab and company pages | AI labs' reports | they replace papers in industry |
| University writing advice | writing centres | they teach IMRaD |

**Strings as run** (web search tool, US-only, standard mode, 2026-10-28; results listed per string in sources.md):

| Id | String |
|---|---|
| G1 | `graphical abstract author guidelines publisher requirements image size` |
| G2 | `plain language summary author instructions journal requirements lay summary` |
| G3 | `data availability statement policy publisher requirement authors "data availability statement"` |
| G4 | `Transparency and Openness Promotion TOP Guidelines 2025 update standards` |
| G5 | `MDAR Materials Design Analysis Reporting framework checklist journals adoption` |
| G6 | `COPE position statement authorship and AI tools` |
| G7 | `ICLR 2026 policy on large language model usage authors reviewers desk rejection` |
| G8 | `ICML 2026 LLM policy authors reviewers call for papers` |
| G9 | `arXiv policy computer science review articles position papers must be peer reviewed generative AI` |
| G10 | `how to write IMRaD paper university writing center guide introduction methods results discussion` |
| G11 | `preprint AI companies publishing research papers 317 firms more than half no paper` |
| G12 | `RRID compliance AACR journals screening tool percent of papers with RRIDs` |
| G13 | `STAR Methods Cell Press key resources table guidelines for authors` |
| G14 | `Springer Nature editorial policies artificial intelligence large language models authorship disclosure copy editing` |
| G15 | `EQUATOR Network reporting guidelines artificial intelligence machine learning TRIPOD-AI CONSORT-AI extension list` |
| G16 | `ACM Artifact Review and Badging version 1.1 Artifacts Available Evaluated Reusable Results Reproduced` |
| G17 | `PLOS author summary guidelines non-technical summary requirement` |

The earlier review's open items gave G5, G9, G11 and G12 (MDAR, the AI-company publishing preprint, the AACR RRID study); the missing TOP and CONSORT-AI gave G4 and G15.

## 6. Stopping rule (Garousi Guideline 8), fixed before searching

- **Effort bounded:** the top 10 results per string, the most the tool returns per call.
- **Saturation:** stop reading a list after 5 consecutive results that add no new concept.
- Applied: every string stopped at its list; G12 and G15 returned two lists, both read.
- G1 and G10 reached saturation: the later results restated the first page (Elsevier's size rule; the same four IMRaD sections).
- Evidence exhaustion was not used: the pool of publisher pages is too large.

## 7. Selection

A grey result is included when it:

- states a rule, a practice or a measurement about article structure, front matter, checklists, availability statements or AI-use rules (IC1);
- comes from the owner or the measurer, not a relay (IC2);
- has a stable address and a date or a stated read date (IC3);
- was read in full, or as a full abstract (IC4);
- scores at least 10 of 20 (section 8).

It is excluded when it:

- is news, a library guide or a blog that restates a rule (EC1);
- is a commercial editing service's page (EC2);
- could not be retrieved, for example by a block or a login redirect (EC3);
- duplicates an included source (EC4);
- concerns only the peer-review process (EC5, out of scope per frame.md).

A source below 10 stays in the review as an **example of practice**; no claim leans on it, and the text that cites it says so.

## 8. Quality of grey sources (Garousi Guideline 11, Table 7)

Twenty criteria, each scored 1, 0.5 or 0; the eight subtotals are in sources.md.

| Criterion | Max | How scored here |
|---|---|---|
| Authority of the producer | 4 | reputable body; author linked to one; author's other work; expertise |
| Methodology | 6 | aim; method stated; references; limits stated; one question; one case |
| Objectivity | 4 | balanced; fact over opinion; no vested interest; conclusions follow data |
| Date | 1 | a stated date |
| Position among related sources | 1 | links to related work |
| Novelty | 2 | adds something; confirms or refutes a position |
| Impact | 1 | the rule governs many venues or papers, or the source is widely used |
| Outlet type | 1 | tier 1 = 1; tier 2 = 0.5; tier 3 = 0 |

- Tier 1: books, standards, reports, white papers, publisher guideline documents. Tier 2: organisers' pages and blog posts, presentations, congress abstracts. Tier 3: personal blogs, e-mail, posts.
- A rule page has no method of its own; the methodology criterion then scores its aim, scope and case only.
- Scores were set by one reader; where a source was not reread in this pass, sources.md says it was scored from the entry in review.md.

## 9. Extraction and synthesis

- Extracted for each source: kind, date, the rule or number stated, who produced it, and whether the producer reports on itself.
- Synthesis is narrative by question (section 2), traceable through sources.md.
- A company or organiser page is its owner's claim about itself; review.md says so in the row.

## 10. Limits

- A second rater re-scored 7 of this topic's grey sources blind ([method](../README.md#method)): all 7 decisions agree. Medawar 1963 is the closest case (11.5 and 10), scored on its catalogue entry by both.
- Search engines personalise and change; the tool returns summaries, so every included source was fetched and read, or its abstract was.
- Pages blocked or redirected to a login were not read: the COPE statement, Springer Nature's AI policy, the ACM badging policy, the PNAS MDAR paper.
- The OpenAlex counts are missing (section 4).
- Some secondary counts are marked "(secondary)" where the primary was not opened (Collberg 2016).
