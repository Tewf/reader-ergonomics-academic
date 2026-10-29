# Academic writing

[![Checks against reader-ergonomics](https://github.com/Tewf/reader-ergonomics-academic/actions/workflows/checks.yml/badge.svg?branch=master)](https://github.com/Tewf/reader-ergonomics-academic/actions/workflows/checks.yml?query=branch%3Amaster)
[![Site](https://github.com/Tewf/reader-ergonomics-academic/actions/workflows/pages.yml/badge.svg)](https://tewf.github.io/reader-ergonomics-academic/)

How to write a report, a research paper, a mathematical article or a proof that meets academic conventions and costs
the reader as little as possible.

It extends [reader-ergonomics](https://github.com/Tewf/reader-ergonomics). The principles, their grades and the checks
live there and are not repeated here. This repository adds only what is particular to these genres: their evidence,
and the shapes of their documents. Where an academic convention and a principle of the standard disagree, the shape
says which one wins, and why.

> **Status:** work in progress. Three multivocal reviews are written and audited in [evidence/](evidence/): research
> papers and mathematical writing, audited on 2026-10-28, and reports. Each of the four shapes has a skeleton, a LaTeX
> version and a worked example; the report shape is a first draft. It is an informal reading of published research and practice: not an
> official standard, not a peer-reviewed study, not a new result, and not a claim to the state of the art.
>
> **How it is made:** with Claude, an AI assistant by Anthropic, under the maintainer's direction, the way
> reader-ergonomics was made. AI agents draft the literature reviews; every reference is resolved by script, and a
> number read only in a summary is marked "(secondary)". Corrections are welcome as issues.

## Scope

Four kinds of document, each with its own evidence and its own shape:

![Academic writing here takes four shapes: the report (course project, internship, master's thesis, technical report), the research paper, the mathematical article and the proof.](readme-scope.svg)

<details>
<summary>Graphviz source</summary>

```dot
// The kinds of academic writing this repository gives a shape to: the figure of README.md.
digraph scope {
  graph [rankdir=TB, nodesep=0.4, ranksep=0.5, bgcolor="white", pad=0.2, fontname="Inter"];
  node  [shape=box, style="rounded,filled", fontname="Inter", fontsize=13, margin="0.2,0.1", penwidth=1.5, fontcolor="#1F2328"];
  edge  [fontname="Inter", fontsize=11, color="#3D434B", fontcolor="#55575F", penwidth=1.3, arrowsize=0.8];
  AW [label=<<b>academic writing</b>>, fillcolor="#FFFFFF", color="#3D434B"];
  RP [label=<<b>the report</b><br/><font point-size="11" color="#55575F">course project, internship,</font><br/><font point-size="11" color="#55575F">master's thesis, technical report</font>>, fillcolor="#E6F2EA", color="#2E7D4F"];
  PA [label=<<b>the research paper</b>>, fillcolor="#E6F2EA", color="#2E7D4F"];
  MA [label=<<b>the mathematical article</b>>, fillcolor="#E6F2EA", color="#2E7D4F"];
  PF [label=<<b>the proof</b>>, fillcolor="#E6F2EA", color="#2E7D4F"];
  AW -> RP;
  AW -> PA;
  AW -> MA;
  AW -> PF;
  {rank=same; RP; PA; MA; PF}
}
```

</details>

## Contents

| Part | Holds | State |
|---|---|---|
| [standard.md](standard.md) | the card: how to use this standard, and which shape for which document | written |
| [AGENTS.md](AGENTS.md) | how to change this repository, for a person or a language model | written |
| [evidence/](evidence/) | three reviews: research papers, mathematical writing, and reports (next row) | written, audited |
| [evidence/reports/](evidence/reports/) | the report as a genre: its standards, its readers and examiners, and where academic convention and the standard conflict | written, audited; a second pass on examiners being merged |
| [shapes/](shapes/) | the skeletons of a research paper, a mathematical article and a proof, each with a worked example | written |
| [shapes/academic-report](shapes/academic-report.md) | one template for the four kinds of report, headings in French and English | first draft, with a worked example of a technical report; its structure was tried once on a private course project report, not published here |

Presentations began here and moved to a repository of their own,
[reader-ergonomics-presentations](https://github.com/Tewf/reader-ergonomics-presentations), on 2026-10-29: the two reviews shared 2 of 370 works.

## Check it

```sh
git clone https://github.com/Tewf/reader-ergonomics
python3 reader-ergonomics/checks/run.py path/to/this/repository
```

CI runs the same checks on every push, and a run fails on any error
([checks.yml](https://github.com/Tewf/reader-ergonomics-academic/blob/master/.github/workflows/checks.yml)). The badge at the top
is the last result on master: the proof that this repository obeys the standard it extends. Every push to master also
renders the site, [tewf.github.io/reader-ergonomics-academic](https://tewf.github.io/reader-ergonomics-academic/)
([pages.yml](https://github.com/Tewf/reader-ergonomics-academic/blob/master/.github/workflows/pages.yml)).

## Licence

Code under the [Apache License 2.0](LICENSE); prose under [CC BY 4.0](LICENSES/CC-BY-4.0.txt). Reuse it as you wish, with
credit to this repository; [CITATION.cff](CITATION.cff) gives a citation if you need one.
