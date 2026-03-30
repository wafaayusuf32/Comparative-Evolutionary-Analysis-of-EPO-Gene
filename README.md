# Comparative Evolutionary Analysis of EPO Gene

## Project Overview
This project explores the evolutionary conservation and divergence of the **Erythropoietin (EPO)** gene across different mammalian species. EPO is a critical hormone produced primarily by the kidneys to regulate red blood cell production.

---

## Phase 1: Pairwise Sequence Alignment (DNA Level)
In the first stage, we compared the full genomic DNA sequences of the **Human** and **Mouse** EPO gene to understand the overall structural similarity.

### Methodology
- **Tool:** EMBOSS Needle (Global Alignment).
- **Algorithm:** Needleman-Wunsch.
- **Data Source:** NCBI (Genomic FASTA).

### Results
- **Length:** 3880 bp
- **Identity:** 1687/3880 (43.5%)
- **Similarity:** 1687/3880 (43.5%)
- **Gaps:** 1730/3880 (44.6%)

### Biological Interpretation
The **43.5% identity** reflects the natural divergence between humans and mice at the genomic level. 
1. **Introns vs. Exons:** The low overall identity is mainly due to the presence of **Introns** (non-coding regions) which accumulate mutations much faster than protein-coding regions.
2. **Structural Differences:** The high percentage of **Gaps (44.6%)** indicates that while the function remains the same, the gene's "architecture" (size and non-coding intervals) has changed significantly throughout evolution.
3. **Conserved Islands:** Despite the low overall score, specific regions show high alignment, representing the essential exons maintained by natural selection for kidney function.
