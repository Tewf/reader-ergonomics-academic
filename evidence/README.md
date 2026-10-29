# Evidence

One literature review per topic, in the steps reader-ergonomics uses for its own
[evidence](https://github.com/Tewf/reader-ergonomics/tree/v1.10.0/evidence): frame, review, state of the art, position, the
case against, baseline. Every work cited is listed once in the [bibliography](bibliography.md).

| Topic | Question |
|---|---|
| [academic-papers](academic-papers/) | how a research article is ordered, what the evidence says about that order, and what templates enforce |
| [mathematical-writing](mathematical-writing/) | how a mathematical article and each proof in it should be laid out for the reader |
| [reports](reports/) | how a course project report, an internship report, a master's thesis and a technical report are ordered, who reads and grades them, and where academic convention and the standard conflict |

## Method

Each topic is a **multivocal literature review**: a review built to a written protocol after Garousi 2019,
which reads together research and **grey literature** (standards, company practice, templates, practitioner books and sites). Two files in each topic make the review checkable and rerunnable:

| File | What it holds |
|---|---|
| `protocol.md` | why grey literature is included, the questions, every search string with its date and count, the stopping rule, the selection criteria |
| `sources.md` | every included source, how it was found, and its quality: the evidence grade for research, a score out of 20 for grey literature |

A grey source is scored on Garousi's 20 criteria, in eight groups. The `sources.md` tables abbreviate these score groups: A authority
(of 4), M methodology (6), O objectivity (4), D date (1), P position among related sources (1), N novelty (2), I impact
(1), T outlet tier (1). A source whose score is below 10 of 20 may illustrate what practice does, but it never supports a claim.

Each review keeps two records apart: **most adopted**, a practice record, and **best evidence**, a research record.
Practice counts as evidence only where a study measured its effect. The formal search of the papers and mathematical-writing topics was
narrative, with snowballing; their protocol files record its terms and counts after the fact, and say so. The grey
search was run to the protocol.

**Second rater.** A second rater re-scored, blind, every fifth grey source (38 of 175) of the seven reviews then in this
repository and of software-design-writing:

- inclusion: the raters agreed for 89.5% of the sample, Cohen's kappa 0.46, unstable at this size (bootstrap 0.00 to 0.87);
- totals: intraclass correlation ICC(A,1) 0.62, mean absolute difference 2.05 of 20, the second rater 1.8 points higher;
- four sources moved from below 10 to above it, and each stays an example of practice;
- the raters differed most on novelty, methodology and objectivity;
- outlet tier was not scored blind, and the first rater kept only the eight subtotals.

## Audit

Every line of the evidence files and shapes that carries a number was checked against its primary
source on 2026-10-28, and every DOI in the bibliography was resolved. Of 72 numeric lines: 53 correct, 11 imprecise, 5 unverifiable,
3 repeating a checked claim, 0 wrong. A second audit, on 2026-10-28, checked the 70 numeric lines added after the first:
50 correct, 14 imprecise, 2 unverifiable, 4 repeats, 0 wrong, all corrected or narrowed.
The presentations review, audited the same day, moved to its own repository,
[reader-ergonomics-presentations](https://github.com/Tewf/reader-ergonomics-presentations), on 2026-10-29.

On 2026-10-28, seventeen claims the audits could not verify were checked against the full texts, which the university's access provided. Of those claims, 9 were correct, 6 imprecise, 1 wrong and 1 still unverifiable, and the files were corrected to match. Some of those claims were on presentations, and moved with that review.

The reports review was written in two passes and audited after each, on 2026-10-29. The first pass: 135 lines, 97
correct, 22 imprecise, 14 unverifiable and 2 wrong. The second, on examiners and on putting the summary first: 101
lines, 62 correct, 21 imprecise, 15 unverifiable and 3 wrong.

Its paywalled sources were then sent to the university's library. Of 25, 20 were read in full and the claims
corrected to match. The other 5 stay marked: a book, a standard, two papers behind a bot check, and one with no access.

Every wrong, imprecise or unverifiable line was corrected, narrowed to what the source supports, or marked "(secondary)" or
"not checked", here and in the shapes that repeat it. Claims without a number have not been audited this way, so such a
claim is only as good as the review that cites it.
