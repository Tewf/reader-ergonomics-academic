# Evidence

One literature review per topic, in the steps reader-ergonomics uses for its own
[evidence](https://github.com/Tewf/reader-ergonomics/tree/master/evidence): frame, review, state of the art, position, the
case against, baseline. Every work cited is listed once in the [bibliography](bibliography.md).

| Topic | Question |
|---|---|
| [presentations](presentations/) | how slides and the spoken talk around them are built so a listener, who cannot set the pace, understands and remembers |

## Method

Each topic is a **multivocal literature review**: research and grey literature ([defined in each frame](presentations/frame.md):
standards, company practice, templates, practitioner books and sites) in one review, built to a written protocol after
Garousi 2019. Two files in each topic make the review checkable and rerunnable:

| File | What it holds |
|---|---|
| `protocol.md` | why grey literature is included, the questions, every search string with its date and count, the stopping rule, the selection criteria |
| `sources.md` | every included source, how it was found, and its quality: the evidence grade for research, a score out of 20 for grey literature |

A grey source is scored on Garousi's 20 criteria (authority, method, objectivity, date, position, novelty, impact,
outlet). Below 10 of 20 it may illustrate what practice does, but it never supports a claim.

Practice counts as evidence only where a study measured its effect. The formal search was narrative, with
snowballing; the protocol records its terms and counts after the fact, and says so. The grey search was run to the
protocol.

## Audit

Not audited yet. Every DOI was resolved against Crossref when the review was written; the numbers are checked against
their primary sources before this branch is merged, as in reader-ergonomics.
