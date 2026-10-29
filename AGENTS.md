# Contributing to this repository

For anyone changing this repository, person or language model. To write a report, a paper, an article or a proof,
read [standard.md](standard.md) instead; this file is about the repository itself. It extends reader-ergonomics
through the interface in that repository's
[extending.md](https://github.com/Tewf/reader-ergonomics/blob/v1.10.0/extending.md), and relies on nothing else there.

## Before writing

1. Read reader-ergonomics' [standard.md](https://github.com/Tewf/reader-ergonomics/blob/v1.10.0/standard.md), then
   this repository's [standard.md](standard.md). A principle that reader-ergonomics holds is linked, never restated.
2. This repository adds shapes and no principles. A shape belongs here only when an academic genre changes a document:
   a convention of the genre, a reader such as an examiner or a referee, a format such as LaTeX.
3. Where a convention of the genre and a principle of the standard disagree, the shape says which one wins, and why.
4. Each shape has three forms: the Markdown skeleton, its LaTeX version, and a worked example from real work. An edit
   to one form is carried to the other two in the same commit.

## Rules for claims

- The rules for claims are reader-ergonomics' own
  ([its AGENTS.md](https://github.com/Tewf/reader-ergonomics/blob/v1.10.0/AGENTS.md#rules-for-claims)): a grade on every
  claim, `Author Year` in the text, one entry in [evidence/bibliography.md](evidence/bibliography.md), evidence against
  kept in `against.md`, "(secondary)" for a number read in a summary.
- A key names one work across the family: before adding one, check it against the other repositories
  (`bibliography-keys` does, in CI).
- A new claim comes from a review in [evidence/](evidence/README.md). A claim no review holds needs a review strand
  first, written to its protocol and audited.

## Before handing back

```sh
python3 <reader-ergonomics>/checks/run.py . --tiers program,meaning     # the standard's checks, on this repository
python3 <reader-ergonomics>/checks/program/standard_card.py . --write   # after the card changes: rebuilds llms.txt
```

- Fix every error. Fix every warning, or say in one line why it is a false match.
- Answer the judgment questions in `checks/judgments.toml`.
- A figure is a Graphviz `.dot` beside its SVG and its page, rendered and folded under the image by
  reader-ergonomics' `checks/figures/render_figure.py`
  ([its figure shape](https://github.com/Tewf/reader-ergonomics-presentations/blob/master/shapes/figure.md)).

## The site

Every push to master renders the site with Quarto, with reader-ergonomics' stylesheet checked out at build time.
