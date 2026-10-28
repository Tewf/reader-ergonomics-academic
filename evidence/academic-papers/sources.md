# Sources

This file lists every source in the pool of this review: the search flow, what was excluded, and one scored row per source; how it was built is in [protocol](protocol.md).

## Flow

Found is the number of results the search listed; read is the number fetched and read, in full or as an abstract; added is the number new to the review.

| String | Found | Read | Added |
|---|---|---|---|
| E1 IMRaD review | 9 | 0 | 0 |
| E2 reporting-guideline endorsement | 9 | 1 | 1 |
| E3 graphical and visual abstracts | 10 | 1 | 1 |
| E4 plain language summaries | 9 | 1 | 2 |
| E5 structured abstracts | 9 | 0 | 0 |
| E6 ML checklists | 9 | 1 | 1 |
| E7 AI policy audits | 9 | 1 | 1 |
| E8 writing-training reviews | 9 | 1 | 1 |
| Lookup: Blanco 2019 | 10 | 1 | 1 |
| G1 graphical abstract guides | 10 | 1 | 1 |
| G2 plain language summary instructions | 9 | 1 | 1 |
| G3 data availability policies | 10 | 0 | 0 |
| G4 TOP guidelines | 10 | 1 | 1 (+2 pointers) |
| G5 MDAR | 10 | 1 | 1 (+1 pointer) |
| G6 COPE | 10 | 0 | 0 |
| G7 ICLR policy | 9 | 1 | 1 |
| G8 ICML policy | 10 | 3 | 3 |
| G9 arXiv policy | 9 | 1 | 1 |
| G10 IMRaD writing advice | 10 | 1 | 1 |
| G11 AI companies publishing | 9 | 1 | 1 |
| G12 RRID at AACR | 19 | 1 | 1 |
| G13 key resources table | 10 | 1 | 1 |
| G14 Springer Nature AI policy | 10 | 0 | 0 |
| G15 EQUATOR AI extensions | 19 | 1 | 1 |
| G16 ACM badging | 9 | 0 | 0 |
| G17 PLOS author summary | 9 | 1 | 1 |
| Total | 265 (83 on existing reviews, 182 grey) | 22 | 23 (+3 pointers) |

Totals by kind: 12 grey sources and 11 formal sources added with a read source, plus 3 formal pointers (Macleod 2021, Nosek 2015, Grant 2024) cited without being read.
The earlier pool of 101 formal and 23 grey sources was built before this pass by narrative search and snowballing; its rows below carry no string id.

## Excluded

| Reason (protocol.md 7) | Examples | Count |
|---|---|---|
| EC1 relay or secondary | news on arXiv's rule and on AI start-ups; library guides on data statements; editing-service blogs on graphical abstracts | not counted one by one |
| EC3 not retrievable | COPE statement on AI authorship (G6); Springer Nature AI policy (G14); ACM badging policy (G16); a news article on AI start-ups (G11) | 4 |
| EC4 duplicate | the ICML policy covered again by news; the Bhavsar audit found by three strings | not counted |
| EC5 peer-review process only | ICLR and ICML reviewer rules beyond what changes authors' work | not counted |

- The numbers from Gainey 2022 were read in a secondary summary and are marked so in review.md.
- The Galipeau 2015 abstract was seen, not its results.

## Pool

The quality column holds the evidence grade for a formal source.
For a grey source it holds the score out of 20 with the eight subtotals A to T defined in the [method](../README.md#method).

Of 35 grey sources, 6 score below 10: Elsevier highlights (9), eLife 2020 (9.5), Octopus (7.5), Elsevier GA 2026 (9), Elsevier KRT 2026 (9.5), GMU 2026 (7.5).
Each is marked in review.md and in the file that leans on it as an example of practice only; none supports a claim.

| Key | Kind | Found via | Quality | Used in |
|---|---|---|---|---|
| Ad Hoc Working Group 1987 | formal | narrative search and snowballing | convention, untested | review, frame |
| Ahmed 2023 | formal | narrative search and snowballing | convention, untested | review |
| Ashurst 2022 | formal | narrative search and snowballing | supported with caveat | review, against |
| Atkinson 1999 | formal | narrative search and snowballing | supported with caveat | review, against |
| Babic 2019 | formal | narrative search and snowballing | supported with caveat | review, position |
| Bazerman 1988 | formal | narrative search and snowballing | supported with caveat | review, against |
| Bommasani 2023 | formal | narrative search and snowballing | measured, descriptive | review |
| Bommasani 2024 | formal | narrative search and snowballing | supported with caveat | review, state-of-the-art, against |
| Booth 1997 | formal | narrative search and snowballing | measured | state-of-the-art, against |
| Boutron 2010 | formal | narrative search and snowballing | measured | against |
| Boyd 2021 | formal | narrative search and snowballing | supported with caveat | review, state-of-the-art, position, against |
| Bredbenner 2019 | formal | narrative search and snowballing | measured | review, state-of-the-art, against, baseline |
| Buckheit 1995 | formal | narrative search and snowballing | convention, untested | review |
| Budgen 2008 | formal | narrative search and snowballing | measured | review, state-of-the-art, position, baseline |
| Buljan 2018 | formal | narrative search and snowballing | measured | review, state-of-the-art, position, against, baseline |
| Chambers 2013 | formal | narrative search and snowballing | convention, untested | review, baseline |
| Chambers 2022 | formal | narrative search and snowballing | supported with caveat | review |
| Chapman 2019 | formal | narrative search and snowballing | measured | review, against |
| Collberg 2016 | formal | narrative search and snowballing | measured | review, against |
| Danchev 2021 | formal | narrative search and snowballing | measured | review, state-of-the-art, position, against, baseline |
| Dodge 2019 | formal | narrative search and snowballing | supported with caveat | review |
| Findley 2016 | formal | narrative search and snowballing | supported with caveat | review, against |
| Frankston 2024 | formal | narrative search and snowballing | supported with caveat | review |
| Gabelica 2022 | formal | narrative search and snowballing | measured | review, state-of-the-art, position, against, baseline |
| Ganjavi 2024 | formal | narrative search and snowballing | measured, descriptive | review, state-of-the-art, position |
| Gebru 2021 | formal | narrative search and snowballing | convention, untested | review |
| Gnewuch 2025 | formal | narrative search and snowballing | measured | review, against |
| Goldberg 2024 | formal | narrative search and snowballing | supported with caveat | review |
| Gopen 1990 | formal | narrative search and snowballing | supported with caveat | review |
| Gross 2002 | formal | narrative search and snowballing | supported with caveat | review |
| Groth 2010 | formal | narrative search and snowballing | convention, untested | review, against |
| Gundersen 2018 | formal | narrative search and snowballing | measured | review |
| Hamilton 2023 | formal | narrative search and snowballing | measured | review, position, against |
| Hardwicke 2018 | formal | narrative search and snowballing | measured | review, state-of-the-art, position, against |
| Hartley 1996 | formal | narrative search and snowballing | supported with caveat (secondary: read in Hartley 2004a) | state-of-the-art, baseline |
| Hartley 1997 | formal | narrative search and snowballing | measured | state-of-the-art, against |
| Hartley 1999 | formal | narrative search and snowballing | supported with caveat | review |
| Hartley 2000 | formal | narrative search and snowballing | measured | state-of-the-art, against, baseline |
| Hartley 2003 | formal | narrative search and snowballing | measured | review, position |
| Hartley 2004a | formal | narrative search and snowballing | measured | review, state-of-the-art, position, against, baseline |
| Hartley 2014 | formal | narrative search and snowballing | supported with caveat | review, against, baseline |
| Haynes 1990 | formal | narrative search and snowballing | supported with caveat | review |
| Hermann 2020 | formal | narrative search and snowballing | supported with caveat | review, against |
| Heumüller 2020 | formal | narrative search and snowballing | measured | review, state-of-the-art, position, against |
| Hill 1982 | formal | narrative search and snowballing | supported with caveat | review, frame |
| Hillier 2016 | formal | narrative search and snowballing | supported with caveat | review |
| Hopewell 2008 | formal | narrative search and snowballing | convention, untested | review, baseline |
| Hopewell 2025 | formal | narrative search and snowballing | convention, untested | review |
| Howitt 2014 | formal | narrative search and snowballing | supported with caveat | against |
| Hubbard 2017 | formal | narrative search and snowballing | supported with caveat | review, state-of-the-art, position, baseline |
| Hyland 2004 | formal | narrative search and snowballing | supported with caveat | review, frame |
| Ibrahim 2017 | formal | narrative search and snowballing | supported with caveat | review, against |
| Jelicic Kadic 2016 | formal | narrative search and snowballing | measured | review, against |
| Kapoor 2023 | formal | narrative search and snowballing | measured | review, against |
| Karačić 2019 | formal | narrative search and snowballing | measured | review, against |
| Kerr 1998 | formal | narrative search and snowballing | supported with caveat | against, frame |
| Kidwell 2016 | formal | narrative search and snowballing | measured | review, state-of-the-art, position |
| Kim 2022 | formal | narrative search and snowballing | supported with caveat | review, position |
| Kobak 2025 | formal | narrative search and snowballing | measured | review, state-of-the-art, position, against, baseline |
| Liang 2024 | formal | narrative search and snowballing | measured, descriptive | review, state-of-the-art, position, against |
| Liang 2025 | formal | narrative search and snowballing | measured | review, state-of-the-art, position, against |
| Lin 2012 | formal | narrative search and snowballing | measured | review, state-of-the-art, position, against |
| Magnusson 2023 | formal | narrative search and snowballing | measured, descriptive | review, state-of-the-art, position, against |
| Markowitz 2024 | formal | narrative search and snowballing | measured | review, state-of-the-art, position, against |
| Mensh 2017 | formal | narrative search and snowballing | convention, untested | review, against |
| Mitchell 2019 | formal | narrative search and snowballing | convention, untested | review |
| Moskovitz 2024 | formal | narrative search and snowballing | measured | review, state-of-the-art, position, against, baseline |
| Nanayakkara 2021 | formal | narrative search and snowballing | supported with caveat | review, against |
| Nicholas 2007 | formal | narrative search and snowballing | supported with caveat | review |
| Nosek 2014 | formal | narrative search and snowballing | convention, untested | review |
| Oska 2020 | formal | narrative search and snowballing | measured | review, state-of-the-art, position, baseline |
| Page 2021 | formal | narrative search and snowballing | convention, untested | review |
| Pferschy-Wenzig 2016 | formal | narrative search and snowballing | supported with caveat | review, position, against |
| Pimentel 2019 | formal | narrative search and snowballing | measured | state-of-the-art, position, against |
| Pineau 2021 | formal | narrative search and snowballing | convention, untested | review, state-of-the-art, position, against, baseline |
| Pitkin 1999 | formal | narrative search and snowballing | measured | state-of-the-art, against, baseline |
| Plavén-Sigray 2017 | formal | narrative search and snowballing | measured | review, state-of-the-art, against, baseline |
| Renear 2009 | formal | narrative search and snowballing | supported with caveat | review, frame |
| Rogers 2021 | formal | narrative search and snowballing | convention, untested | review |
| Saucez 2019 | formal | narrative search and snowballing | measured, descriptive | review |
| Scheel 2021 | formal | narrative search and snowballing | measured | state-of-the-art, position, against |
| Schulz 2010 | formal | narrative search and snowballing | convention, untested | review |
| Sharma 2006 | formal | narrative search and snowballing | measured | review, baseline |
| Simera 2010 | formal | narrative search and snowballing | convention, untested | review |
| Soderberg 2021 | formal | narrative search and snowballing | measured | state-of-the-art, position |
| Sollaci 2004 | formal | narrative search and snowballing | measured | review, state-of-the-art, position, baseline |
| Stodden 2018 | formal | narrative search and snowballing | measured | review, state-of-the-art, position, against |
| Swales 1990 | formal | narrative search and snowballing | supported with caveat | review, frame |
| Swales 2004 | formal | narrative search and snowballing | supported with caveat | review, position |
| Swales 2012 | formal | narrative search and snowballing | convention, untested | review |
| Sword 2012 | formal | narrative search and snowballing | supported with caveat | review, against |
| Taddio 1994 | formal | narrative search and snowballing | measured | review, state-of-the-art, position, baseline |
| Tenopir 2008 | formal | narrative search and snowballing | supported with caveat | review, state-of-the-art, position |
| Tenopir 2015 | formal | narrative search and snowballing | supported with caveat | review |
| Timperley 2021 | formal | narrative search and snowballing | supported with caveat | review, against |
| Turner 2012 | formal | narrative search and snowballing | measured | review, state-of-the-art, position, baseline |
| Vasilevsky 2013 | formal | narrative search and snowballing | measured | review, position |
| Wang 2024 | formal | narrative search and snowballing | measured | review |
| Weinberger 2015 | formal | narrative search and snowballing | supported with caveat | review, against |
| Winter 2022 | formal | narrative search and snowballing | measured | review, state-of-the-art, position, against, baseline |
| Yang 2016 | formal | narrative search and snowballing | supported with caveat | review, position |
| Stevens 2014 | formal (added) | E2 | measured | review, state-of-the-art, position, against, baseline |
| Blanco 2019 | formal (added) | lookup after E2 | measured, descriptive | review, position, against, frame |
| Galipeau 2015 | formal (added) | E8 | supported with caveat | review, frame |
| Stoll 2022 | formal (added) | E4 | measured | review, state-of-the-art, position, against, baseline |
| Gainey 2022 | formal (added) | E4 | measured, descriptive | review, state-of-the-art |
| Krukowski 2023 | formal (added) | E3 | supported with caveat | review, position |
| Bhavsar 2025 | formal (added) | E7 | measured, descriptive | review, state-of-the-art, position |
| Liu 2020 | formal (added) | G15 | convention, untested | review |
| Macleod 2021 | formal (added) | G5 (pointer, not read) | convention, untested | review |
| Nosek 2015 | formal (added) | G4 (pointer, not read) | convention, untested | review |
| Grant 2024 | formal (added) | G4 (pointer, not read) | convention, untested | review |
| Coakley 2026 | formal (added) | E6 | supported with caveat | review, state-of-the-art, position, against |
| Kim 2026 | formal (added) | G8 | supported with caveat | review, state-of-the-art, position, against |
| Loisel 2026 | formal (added) | G11 | supported with caveat | review, state-of-the-art |
| ICMJE (structure) | grey tier 1 | narrative search | A4 M3 O1.5 D0.5 P0.5 N1 I1 T1 = 12.5/20; scored from the entry in review.md | review, position, against, baseline |
| ICMJE 2023 | grey tier 1 | narrative search | A4 M3 O1.5 D0.5 P0.5 N1 I1 T1 = 12.5/20 | review, position |
| Gastel 2016 | grey tier 1 | narrative search | A4 M4 O3 D1 P1 N0.5 I1 T1 = 15.5/20 | review |
| Elsevier highlights | grey tier 2 | narrative search | A3.5 M2.5 O1 D0 P0 N0.5 I1 T0.5 = 9/20 (below 10: example of practice only); scored from the entry in review.md | review, against, frame |
| Marcus 2016 | grey tier 1 | narrative search | A4 M3 O1 D1 P0.5 N1 I1 T1 = 12.5/20 | review |
| eLife 2017 | grey tier 2 | narrative search | A3.5 M4.5 O1 D1 P0.5 N1 I0.5 T0.5 = 12.5/20 | review, against |
| eLife 2020 | grey tier 2 | narrative search | A3.5 M2 O1 D1 P0 N1 I0.5 T0.5 = 9.5/20 (below 10: example of practice only) | review, position |
| Octopus | grey tier 2 | narrative search | A3 M2 O1 D0 P0 N0.5 I0.5 T0.5 = 7.5/20 (below 10: example of practice only); scored from the entry in review.md | review |
| Olah 2017 | grey tier 1 | narrative search | A3.5 M2 O2 D1 P0.5 N1 I1 T1 = 12/20 | review |
| Distill 2021 | grey tier 2 | narrative search | A3.5 M2 O2 D1 P0.5 N0.5 I0.5 T0.5 = 10.5/20 | against |
| Nature 2023 | grey tier 1 | narrative search | A4 M2.5 O1.5 D1 P0.5 N1 I1 T1 = 12.5/20 | review, position |
| ACL 2023 | grey tier 2 | narrative search | A3.5 M3 O1.5 D1 P0.5 N1 I1 T0.5 = 12/20 | review, position, baseline |
| ICML 2023 | grey tier 2 | narrative search | A3.5 M2.5 O1.5 D0.5 P0.5 N1 I1 T0.5 = 11/20 | review, position |
| NeurIPS 2021 | grey tier 2 | narrative search | A3.5 M3 O1.5 D0.5 P0.5 N1 I1 T0.5 = 11.5/20 | review |
| NeurIPS 2025 | grey tier 2 | narrative search | A3.5 M3 O1.5 D0 P0.5 N1 I1 T0.5 = 11/20; undated | review, position |
| NeurIPS 2026 | grey tier 2 | narrative search | A3.5 M3 O1.5 D0.5 P0.5 N1 I1 T0.5 = 11.5/20; page replaced each year | review, state-of-the-art, baseline |
| OpenAI 2023 | grey tier 1 | narrative search | A4 M4.5 O1 D1 P0.5 N1 I1 T1 = 14/20; owner's account | review, against |
| Rodriguez 2021 | grey tier 1 | narrative search | A3.5 M3 O2 D1 P0.5 N0.5 I0.5 T1 = 12/20 | review, against |
| Pinker 2014 | grey tier 1 | narrative search | A4 M2.5 O2 D1 P0.5 N1 I1 T1 = 13/20 | review |
| Keshav 2007 | grey tier 1 | narrative search | A4 M2 O2 D1 P0.5 N1 I1 T1 = 12.5/20 | review, against |
| Medawar 1963 | grey tier 1 | narrative search | A4 M2 O1.5 D1 P0 N1 I1 T1 = 11.5/20; essay in a magazine | against |
| CTAN class documentation (elsarticle, llncs, IEEEtran, acmart) | grey tier 2 | narrative search | A3.5 M2 O2 D0.5 P0 N0.5 I1 T0.5 = 10/20; scored as one group, from the entries in review.md | review |
| JATS | grey tier 1 | narrative search | A4 M3 O2 D1 P0.5 N1 I1 T1 = 13.5/20; scored from the entry in review.md | review, frame |
| Elsevier GA 2026 | grey tier 2 (added) | G1 | A3.5 M2.5 O1 D0 P0 N0.5 I1 T0.5 = 9/20 (below 10: example of practice only); undated | review, against |
| Elsevier KRT 2026 | grey tier 2 (added) | G13 | A3.5 M2.5 O0.5 D0 P0.5 N1 I1 T0.5 = 9.5/20 (below 10: example of practice only); undated; claims without data | review, position, against |
| Taylor & Francis 2024 | grey tier 1 (added) | G2 | A3.5 M3 O1 D1 P0.5 N1 I0.5 T1 = 11.5/20 | review, position, baseline |
| PLOS 2026 | grey tier 2 (added) | G17 | A3.5 M3 O1.5 D0 P0 N0.5 I1 T0.5 = 10/20; undated | review, position, baseline |
| ICLR 2025 | grey tier 2 (added) | G7 | A3.5 M3.5 O1.5 D1 P1 N1 I1 T0.5 = 13/20 | review, position |
| ICML 2026a | grey tier 2 (added) | G8 | A3.5 M3 O1.5 D0 P0.5 N1 I1 T0.5 = 11/20; undated | review |
| ICML 2026b | grey tier 2 (added) | G8 | A3.5 M4.5 O1.5 D1 P1 N1.5 I1 T0.5 = 14.5/20; owner's account | review, state-of-the-art, position, against |
| arXiv 2025 | grey tier 2 (added) | G9 | A3.5 M3.5 O1.5 D1 P0.5 N1 I1 T0.5 = 12.5/20 | review, position |
| COS 2024 | grey tier 2 (added) | G4 | A3.5 M3 O1.5 D1 P0.5 N1 I1 T0.5 = 12/20; owner's account | review |
| COS 2019 | grey tier 2 (added) | G5 | A3.5 M3.5 O1 D1 P0.5 N1 I0.5 T0.5 = 11.5/20; owner's account | review |
| GMU 2026 | grey tier 2 (added) | G10 | A2.5 M2 O1.5 D0 P0.5 N0 I0.5 T0.5 = 7.5/20 (below 10: example of practice only); undated | review |
| Evanko 2025 | grey tier 2 (added) | G12 | A3.5 M4.5 O1.5 D1 P0.5 N1.5 I0.5 T0.5 = 13.5/20; owner's data | review, state-of-the-art, position, baseline |
