# Frame: the problem and the field's names for it

This file states the problem in one sentence and lists what mathematics and its education research call its parts.

## The problem in one sentence

How should one lay out a mathematical research article, and each proof inside it, so that a reader finds the result, judges whether it holds, and sees why it holds, at the least reading cost?

## Five sub-questions

| Id | Sub-problem | Unit |
|---|---|---|
| Q1 | The order and kinds of sections in a mathematics article | article |
| Q2 | Where the main results are stated | article |
| Q3 | How a single proof is laid out: paragraph, numbered hierarchy, calculation | proof |
| Q4 | Whether a layout changes what readers understand, and how that is measured | reader |
| Q5 | Whether the dependencies between lemmas are made explicit | article and proof |

## What each field calls it

The problem is shared by five fields, and each one names it differently.

| Field | Names for the problem | Key source |
|---|---|---|
| Style guides by mathematicians | **mathematical writing**, **mathematical exposition** | Halmos 1970, Knuth 1989, Krantz 2017, Higham 2020 |
| Applied linguistics | **genre analysis**, **move analysis**, the **CARS model** (Create a Research Space), **macrostructure**, **IMRD** versus **Introduction-Results** | Swales 2004, Graves 2013, Kuteeva 2015 |
| Philosophy of mathematical practice | the **definition-theorem-proof (DTP) model**, **explanatory proof** | Thurston 1994, Steiner 1978, Hanna 1990 |
| Mathematics education | **proof comprehension**, **proof reading**, **proof validation**, **proof presentation**, **modular reading**, **self-explanation**, **e-Proofs**, **generic proof** | Mejia-Ramos 2012, Selden 2003, Weber 2011, Hodds 2014, Roy 2017b, Leron 2013 |
| Computer science and formal methods | **structured proof**, **hierarchical proof**, **calculational proof**, **structured derivation**, **declarative proof**, **blueprint**, **dependency graph** | Lamport 1995, Dijkstra 1990, Back 2010, Wenzel 1999, leanblueprint |

## Method: a multivocal literature review

This review is a **multivocal literature review (MLR)** (Garousi 2019; defined in the [evidence README](../README.md)): it reads together the formal literature and the **grey literature** (sources outside journals and academic presses). Grey sources are sorted into **tiers** by outlet control.

| Tier | Outlet control | Examples here |
|---|---|---|
| 1 | high | books, publishers' and societies' author rules |
| 2 | moderate | university handouts, videos, Q/A threads, project documentation |
| 3 | low | blogs |

The method is in protocol.md and the scored pool in sources.md.

## What practitioners call it

| Practitioners' word | The field's word |
|---|---|
| advice on writing papers; selling the key points | announcing principal findings |
| milestones; create lemmas | modular structure (Mejia-Ramos 2012) |
| high-level overview; proof outline | proof sketch; summary of high-level ideas |
| module docstring; main statements | none in the formal literature |
| postponing a proof | none in the formal literature |

## Terms defined before use

- **Move**: a stretch of text with one rhetorical function, such as announcing the findings (Swales 2004).
- **DTP model**: the picture of mathematics as definitions, then theorems, then deductive proofs; the name is from Thurston 1994.
- **Linear proof**: a proof written as consecutive paragraphs of prose, the default in journals.
- **Structured proof**: a proof split into levels, each step numbered and given its own justification (Leron 1983 for communication, Lamport 1995 for rigor).
- **Calculational proof**: a chain of expressions joined by relations, each link carrying a hint in braces (Dijkstra 2000).
- **Proof comprehension**: what a reader can answer about a proof after reading it, along local and holistic dimensions (Mejia-Ramos 2012).
- **Warrant**: the reason that licenses one line of a proof to follow from earlier ones; often left implicit (Inglis 2012).
- **Blueprint**: a human-readable proof outline whose statements declare which earlier statements they use, so a dependency graph can be drawn (leanblueprint, Massot 2026).

## Our words against the field's words

| Our word | The field's word |
|---|---|
| article template | macrostructure; genre conventions |
| results early | announcing principal findings (Move 3 of CARS) |
| proof sketch first | proof sketch (Lamport 2012); summary of high-level ideas (Mejia-Ramos 2012) |
| numbered steps | hierarchical structured proof |
| explicit dependency tree | dependency graph (blueprint); modular structure (Mejia-Ramos 2012) |

## Search terms used three ways

- Academic name: "proof comprehension", "structured proofs", "genre analysis mathematics research articles", "definition-theorem-proof".
- Acronym: DTP, CARS, IMRD, PFR, MSC.
- Author: Lamport, Leron, Thurston, Weber, Mejia-Ramos, Inglis, Alcock, Kuteeva, Graves, Massot.
- Grey strings are listed in protocol.md 5.
