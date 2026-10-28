# Baseline

This file names the baseline a proposed paper shape is compared against, and how the comparison would be measured.

## The named baseline

**IMRaD with a structured abstract**: Introduction, Methods, Results, Discussion; an abstract labelled Background, Methods, Results, Conclusions; and the EQUATOR reporting checklist for the study design when one exists.

Why this one:

- It is the control condition in the structured-abstract studies cited here (Hartley 2004a, Taddio 1994, Budgen 2008).
- It is what ICMJE asks of original research (ICMJE 2026), and what the leading medical journals print (Sollaci 2004).
- Readers and reviewers already know where to look in it, so any new shape must beat it, not merely differ from it.
- Its checklist part rests on CONSORT evidence; for other guidelines endorsement showed no significant gain on nearly every item (Stevens 2014).

## A second named baseline, for computing and ML papers

**IMRaD with a structured abstract, the venue checklist (NeurIPS or ACL) filled in, a data and code statement with a persistent archive, and a one-line language-model use declaration where the venue asks.**

Why: it is what an author at these venues actually submits (NeurIPS 2026, ACL 2023), so a proposed shape for those venues must beat it. The first baseline stays the control for medicine and other fields.

## What to measure

| Outcome | Definition | Instrument used before | Source |
|---|---|---|---|
| Time to find a result | seconds from question to correct answer | timed true/false questions on screen | Hartley 1996 |
| Retrieval accuracy | share of questions answered correctly | same | Hartley 1996 |
| Comprehension | score on questions about the claim, the method and one limitation, graded blind | written questions | no prior instrument found for full articles |
| Recall | delayed free recall scored against the main ideas | recall test | Hartley 2004a, study 18 |
| Information content of the abstract | items present over items applicable, from 0 to 1 | 33-criterion or 29-item checklist; CONSORT for abstracts | Taddio 1994; Sharma 2006; Hopewell 2008 |
| Fidelity | abstract data present in and consistent with the body | audit against the body | Pitkin 1999 |
| Completeness of reporting | share of guideline items reported | CONSORT or PRISMA items | Turner 2012 |
| Judged clarity | rating from 1 to 10 by independent researchers | paired rating | Budgen 2008 |
| Readability, secondary only | FRE and NDC scores | formula | Plavén-Sigray 2017 |
| Checklist accuracy | share of yes answers a reader can confirm in the paper | reviewer check of code claims | Pineau 2021 |
| Artifact reachability | share of artifact links that work after N years | automated link check | Winter 2022 |
| Declared against actual availability | share of data and code statements that lead to usable files | statement audit and retrieval | Danchev 2021, Gabelica 2022 |
| Knowledge from a summary | score on questions about the findings after reading a summary | multiple-choice knowledge test | Buljan 2018 |
| Perceived understanding | self-rated understanding after the summary | survey item | Bredbenner 2019 |
| Compliance after a prompt | share of articles meeting a requirement after an automated reminder at a set editorial point | before and after at one publisher | Evanko 2025 |
| Language-model signature | excess-vocabulary share in the abstract, as a covariate | word-frequency comparison | Kobak 2025 |

## How to compare

- Write the same study in both shapes, by someone other than the experimenter, to avoid the rewriting bias described in Hartley 2014.
- Hold length constant or report it, since length alone produced advantages in Hartley 2004a.
- Use a within-subject crossover with counterbalanced order, as in Budgen 2008 and Oska 2020.
- Recruit novices and experienced researchers separately, since they read different parts (Hubbard 2017).
- Cover at least two fields, since effects differed by discipline (Hartley 2000, Moskovitz 2024).
- Preregister the protocol, Registered Report style (Chambers 2013).
- Report effect sizes with intervals, and publish the questions and the texts.
- Report whether the texts were written or edited with a language model, and the excess-vocabulary share, since 13.5% or more of 2024 biomedical abstracts show it (Kobak 2025).

## Not baselined

- Highlights, graphical abstracts and the CARS order have no reader study against this baseline; they stay convention, untested.
- Model cards, datasheets, STAR Methods, significance statements and release blog posts have no reader study against either baseline; they stay convention, untested.
- Plain-language summary formats (Taylor & Francis 2024, PLOS 2026) have publisher rules and no comparison against the abstract on knowledge (Stoll 2022, Buljan 2018).
