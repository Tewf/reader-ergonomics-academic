# Position: what is known, what is not, what this repository adds

This file sets out what is known, what is not, and what this repository adds about mathematical articles and proofs.

## Known

| Claim | Grade | Source |
|---|---|---|
| Mathematics articles use Introduction-Results, not IMRD | measured, descriptive | Graves 2013, Kuteeva & McGrath 2015 |
| Openings almost always announce the principal findings | measured, descriptive | Kuteeva & McGrath 2015 |
| Expert guides agree that the main results go first, stated as self-contained sentences | convention, untested | Halmos 1970, Knuth 1989, Krantz 2017, Tao 2026a |
| A Leron-style structured proof helps readers grasp the summary and may cost local detail | measured, one study | Fuller 2014 |
| More presentation support can lower retention | measured, one study | Roy 2017b |
| Training the reader to self-explain raises comprehension by about one standard deviation | measured, replicated by the same team | Hodds 2014, Alcock 2015 |
| Experts spend their effort on implicit warrants between lines | measured | Inglis & Alcock 2012 |
| Mathematicians do not share one standard of validity | measured | Inglis 2013b |
| Formalisation through a blueprint exposes missing hypotheses | supported with caveat (case reports) | Tao 2023 |

## Not known

- Whether stating the main theorem early changes what readers understand or decide; no experiment was found.
- Whether Lamport's numbered format helps readers, as opposed to helping its writer find errors.
- Whether proof depth matters: no study varies the number of levels.
- Whether an explicit dependency list or graph helps a human reader, rather than a proof assistant.
- Whether Fuller 2014 replicates: we found no second study of structured versus linear proofs.
- Whether results from undergraduates hold for research mathematicians reading in their own field.

## Positioned against the existing reviews

| Review | Covers | Leaves open |
|---|---|---|
| Stylianides 2024, Stylianides 2017, Lessing 2025 | proof and proving in education | how a text is laid out for its reader |
| Teledahl 2024, Powell 2017 | the quality of students' mathematical writing | the research article and its readers |
| Tran Minh 2025 | proof assistants in teaching | blueprints as structure for human readers |

This search did not find a review that compares layouts of a research article or a proof, so this repository's contribution is a comparison across both communities, not a replacement of those reviews.

## Where practice runs ahead of the evidence

- Every guide puts the main results in the introduction; no experiment tests it (state-of-the-art.md Q2).
- About 40 formalisation projects list a blueprint with its `uses` labels; no study asks whether the graph helps a human reader.
- Publishers enforce rules of form (abstract without citations, theorem styles); none of the rules was tested.
- Practitioners disagree on postponing proofs (Ilmavirta 2015); no evidence settles it.

## Where evidence is ignored by practice

- Self-explanation training (Hodds 2014, d = 0.95) appears in none of the guides found.
- Roy 2017b warns that narrated support can lower retention; none of the guides found mentions it.

## "Nobody has done it" versus "we have not seen it"

- Every gap above is a statement about our search, not about the world.
- Searched: the three-way terms in frame.md on the web and on arXiv.
- Then forward from Leron 1983 and Mejia-Ramos 2012 through the works that cite them.
- Then the grey strings of protocol.md 5 and four searches for existing reviews.
- A thesis titled "Tools for semi-formal proofs", listed in the Texas Digital Library, reports an experiment against prose proofs; its record could not be opened, so it is the first lead to chase.

## What this repository adds

Two templates, under `shapes/`, that combine the convention with the one measured trade-off.

| Rule in the templates | Why | Grade of the support |
|---|---|---|
| Abstract, MSC code, introduction stating the main theorem in section 1 | the field's genre and publisher rules | measured, descriptive; enforced |
| Section plan: introduction, preliminaries, results, proofs, references | Krantz 2017 and the corpus stages of Kuteeva & McGrath 2015 | convention, untested |
| Each proof opens with a one-paragraph sketch | serves the holistic dimension that structure helped | measured, one study (Fuller 2014) |
| Then numbered steps, each with its own justification | serves the local dimension that a bare structure risked losing; makes warrants explicit | supported with caveat (Inglis & Alcock 2012, Fuller 2014) |
| At most three levels, about 4 to 10 steps each | Lamport 2012's readability limit; shallow trees keep step names readable | convention, untested |
| Each lemma lists the results it uses | the blueprint practice; Tao's box-and-arrow drawing | convention, untested for human readers |
| A paragraph proof is kept when the argument is short or a single idea | Lamport 2012 uses structure only above about ten lines; Fuller 2014 found costs | supported with caveat |

The repository's claim is narrow: these templates are a hypothesis, to be tested against the baseline in baseline.md.
