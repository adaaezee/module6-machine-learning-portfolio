# Unit 5 - Clustering

[← Back to e-portfolio](../README.md) · **LO1, LO2**

**Artefact:** Jaccard distance calculations (e-portfolio activity)

Clustering depends on how "distance" between records is defined. For three patients' test results, I removed Gender, because it is a symmetric attribute and Jaccard distance is designed for asymmetric ones, where only a positive result carries information. I then coded Y and P as 1, and N and A as 0, assuming "A" means absent.

| | Fever | Cough | Test-1 | Test-2 | Test-3 | Test-4 |
|---|---|---|---|---|---|---|
| Jack | 1 | 0 | 1 | 0 | 0 | 0 |
| Mary | 1 | 0 | 1 | 0 | 1 | 0 |
| Jim | 1 | 1 | 0 | 0 | 0 | 0 |

Jaccard distance is d = (r + s) / (q + r + s), where q counts attributes positive for both people, r and s count those positive for only one, and shared negatives are ignored.

| Pair | q | r | s | Distance |
|---|---|---|---|---|
| Jack, Mary | 2 | 0 | 1 | 1/3 = **0.33** |
| Jack, Jim | 1 | 1 | 1 | 2/3 = **0.67** |
| Jim, Mary | 1 | 1 | 2 | 3/4 = **0.75** |

Jack and Mary are the most similar, and Jim and Mary the least.

**What I learned:** the choice of distance measure is a judgement about what the data means. Ignoring shared negatives suits medical tests, where two healthy results say little. Coding the undefined "A" value was an assumption that could change the results, which is a data-quality risk. Excluding gender also avoids grouping patients by a sensitive attribute with no clinical relevance here. I applied the same idea of evaluating clusters carefully when choosing *k* in the [team project](../projects/unit-06-team-project/).

**AI use:** Calculations checked with AI assistance (ChatGPT).
