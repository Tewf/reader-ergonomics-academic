# The academic writing standard

What a report, a research paper, a mathematical article and a proof need beyond what any text needs: the conventions
of each genre, the evidence behind them, and a shape for each. It extends
[reader-ergonomics](https://github.com/Tewf/reader-ergonomics/blob/v1.18.2/standard.md), the standard for any reader:
read that one first.

## How to use it

1. **Pick the shape** of the document in [shapes/](shapes/README.md). Each shape gives a skeleton, a LaTeX version
   and a worked example.
2. **Write to the principles** of reader-ergonomics, which all hold here. Where an academic convention disagrees with
   one, the shape says which wins, and why.
3. **Check:** run `python3 <reader-ergonomics>/checks/run.py .` on the folder. Fix each error, fix or explain each
   warning, and answer each judgment in `checks/judgments.toml`.

## Principles

This extension adds shapes and no principles. The principles are reader-ergonomics' own, listed with their grades in
[its card](https://github.com/Tewf/reader-ergonomics/blob/v1.18.2/standard.md#principles).

## Shapes

| Document | Shape |
|---|---|
| a course project report, an internship report, a master's thesis, a technical report | [academic report](shapes/academic-report.md) |
| an empirical study for a journal, a conference or a preprint server | [research paper](shapes/research-paper.md) |
| a proof-centred mathematics article | [mathematical article](shapes/mathematical-article.md) |
| one long proof in numbered steps | [proof](shapes/proof.md) |

## Evidence

Each shape rests on a review in [evidence/](evidence/README.md), and every work cited is listed once in the
[bibliography](evidence/bibliography.md).
