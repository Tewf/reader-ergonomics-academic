# Position

This file states what the evidence settles, what it leaves open, and what this repository adds.

## Known

- Reporting checklists raise completeness, modestly and unevenly (Turner 2012). Grade: measured.
- Structured abstracts hold more information than unstructured ones in medicine, psychology and software engineering (Taddio 1994, Hartley 2003, Budgen 2008). Grade: measured.
- Accepting the question and method before results changes what gets published (Scheel 2021, Soderberg 2021). Grade: measured.
- Researchers read many articles, briefly and by parts; experienced readers go to figures and results (Tenopir 2008, Hubbard 2017). Grade: supported with caveat.
- IMRaD dominates biomedicine and is not universal elsewhere (Sollaci 2004, Lin 2012, Moskovitz 2024). Grade: measured.
- A required checklist is filled in by nearly every author and changes some reporting; self-reported answers overstate (Pineau 2021, Magnusson 2023). Grade: measured, descriptive.
- Artifact badges go with artifacts that stay reachable, not with more citations (Winter 2022, Heumüller 2020). Grade: measured.
- A statement that data or code exist is a weak signal of real availability (Danchev 2021, Gabelica 2022, Hamilton 2023). Grade: measured.
- Mandates and badges raise sharing where they are tied to a visible act (Hardwicke 2018, Kidwell 2016). Grade: measured.
- A plain-language text is simpler than the abstract, with small effects; it did not beat another text summary on knowledge (Markowitz 2024, Buljan 2018). Grade: measured.
- A large share of recent biomedical and computer science abstracts show language-model signatures (Kobak 2025, Liang 2025). Grade: measured.

## Not known

- Whether IMRaD lets a reader find or understand a result faster than another order. Hartley 2004a reported that no study had compared complete articles in either format, and this review found none since. That is a statement about this search, not a claim that no such study exists.
- Whether highlights help readers: we found genre analyses (Yang 2016) and publisher guidance, no reader study.
- Whether graphical abstracts improve understanding: the studies found measure attention or citations (Oska 2020, Pferschy-Wenzig 2016, Kim 2022).
- Whether the CARS or hourglass order improves comprehension: move studies describe expert practice (Swales 2004).
- Whether executable articles are read or trusted differently: we found reproducibility audits (Pimentel 2019) and platform reports (eLife 2020), no reader study.
- Whether any ML checklist improved the quality of published work: its organisers said they had no evidence (Pineau 2021), and the later analysis is of self-reports (Magnusson 2023).
- Whether STAR Methods or a key resources table improved reporting: this search found related identifier studies (Vasilevsky 2013, Babic 2019), none of the format.
- Whether reading a paper with a significance statement beats reading it without: the studies found compare statements with abstracts or with model-written ones.
- Whether model cards and datasheets are used as intended: the one user test is small (Boyd 2021).
- How blog posts and technical reports from companies are read and cited against papers: this search did not find it.
- Whether disclosure rules track use: this search did not find a study.

## Where practice runs ahead of the evidence

- Language-model rules (Nature 2023, ICMJE 2023, ACL 2023, ICML 2023) were published in 2023; the first population-level estimates are from 2024 (Liang 2025, Kobak 2025).
- Checklists were mandatory at NeurIPS from 2019 and at ACL venues from 2020; the first analysis of a venue-wide checklist is from 2023 (Magnusson 2023).
- STAR Methods, significance statements and digests are standard formats; the tests found compare summary formats, not the journal's own.
- Model cards are the default documentation on a major model hub (Liang 2024); the controlled evidence is one think-aloud study and a small intervention.

## Where the evidence is ignored by practice

- "On reasonable request" remains the most common statement in one large audit (42%, Gabelica 2022), though request-based retrieval gave 6.8% there and 44% in Stodden 2018.
- Venue policies on language-model use differ and sometimes conflict with the publisher's (12 journals, Ganjavi 2024), and writing-only use may need no declaration (NeurIPS 2025), so disclosure cannot calibrate an estimate of use. This last point is an inference from the two sources.

## What this repository adds

- No new data.
- A shape, [research-paper](../../shapes/research-paper.md), that keeps the baseline and labels each part with its grade.
- Additions to the baseline only where evidence exists elsewhere. They are a structured abstract with numbers, a named reporting checklist, the plan with its deviations (from Registered Reports), and a data and code statement (from reproducible research).
- Parts with no reader evidence (highlights, graphical abstract, the CARS order) stay optional and marked convention, untested.
- A protocol (baseline.md) so a future study can test a proposed shape against IMRaD on reader outcomes.
- A reporting-checklist row that names the venue checklist where one exists (NeurIPS, ACL), beside the EQUATOR one.
- A data and code statement that gives a persistent archive and a version, not "on request" (Gabelica 2022, Danchev 2021).
- An AI-use declaration row, grade convention, untested, worded to the venue's rule.
- Plain-language summaries and significance statements stay optional, convention, untested for reader benefit.

