# Dataset Inventory and License Audit

All datasets used in this project are publicly available or community-authorized.
No private, restricted, or culturally sensitive materials are used without explicit community permission.

---

## Cree Sources

| Title | Dialect | Type | License | Training Safe | URL |
|---|---|---|---|---|---|
| Bloomfield Plains Cree Texts (1934) | Plains Cree (y-dialect) | Text Corpus | Public Domain |  Yes | https://archive.org/details/rosettaproject_crk_vertxt-2 |
| Sacred Stories of the Sweet Grass Cree (1930) | Plains Cree (y-dialect) | Bilingual Text Corpus | Public Domain | Yes* | https://archive.org/details/P005409 |
| A Dictionary of the Cree Language (Faries, 1938) | Multi-dialect (Swampy/Moose primary) | Dictionary | Public Domain | Yes | https://www.torontopubliclibrary.ca |
| A Dictionary of the Cree Language (Watkins, 1865) | Swampy Cree (n-dialect) | Dictionary | Public Domain | Yes | https://archive.org/details/dictionaryofcree00watk |
| A Grammar of the Cree Language (Howse, 1844) | Swampy Cree (n-dialect) | Grammar | Public Domain |Yes | https://archive.org/details/agrammarcreelan02howsgoog |

*Bloomfield Sacred Stories: training-safe but avoid generating synthetic sacred stories in the same tradition or reframing cultural narratives without community review.

### Dialect Note
Faries (1938), Watkins (1865), and Howse (1844) cover Swampy, Moose, and East Cree dialects — not Plains Cree. Only Bloomfield (1930, 1934) are confirmed Plains Cree (y-dialect). This distinction is reflected in dataset labeling.

---

## Ojibwe Sources

| Title | Dialect | Type | License | Training Safe | URL |
|---|---|---|---|---|---|
| A Dictionary of the Otchipwe Language Part I (Baraga, 1878) | Southwestern Ojibwe | Dictionary | Public Domain | Yes | https://archive.org/details/cihm_61742 |
| A Dictionary of the Otchipwe Language (Baraga, 1853) | Southwestern Ojibwe | Dictionary | Public Domain | Yes | https://archive.org/details/adictionaryotch00baragoog |
| A Theoretical and Practical Grammar of the Otchipwe Language (Baraga, 1878) | Southwestern Ojibwe | Grammar | Public Domain | Yes | https://archive.org/details/cihm_07287 |
| Ojibwa Texts (Jones & Michelson, 1917) | Southwestern Ojibwe | Historical Texts | Public Domain | Yes | https://archive.org/details/ojibwatextsvolu00michgoog |

### Excluded Sources
| Title | Reason |
|---|---|
| Ojibwe People's Dictionary | CC BY-NC-SA 3.0 — NC clause blocks ML training |
| Cree Language of the Plains Textbook | CC BY-NC-ND 4.0 — NC-ND blocks ML training and dataset derivation |
| Ojibwe Vocabulary and Grammar (Lockwood) | CC BY-NC-ND 3.0 — NC-ND blocks ML training |

---

## Inuktitut Sources

| Title | Dialect | Type | License | Training Safe | URL |
|---|---|---|---|---|---|
| EdinburghNLP Nunavut Hansard++ | Baffin Island / Nunavut dialects | Parallel Corpus | CC BY 4.0 | Yes | https://huggingface.co/datasets/EdinburghNLP/nunavut-hansard-plusplus |

Attribution required. Must not be used to misrepresent statements of Nunavut legislators.

---

## Training Dataset Summary

| Language | Entries | Sources |
|---|---|---|
| Plains Cree | 2,241 | 5 sources |
| Ojibwe | 2,057 | 4 sources |
| Inuktitut | 4,937 | 1 source (Hansard) |
| **Total** | **9,235** | **10 sources** |

Last updated: June 2026
