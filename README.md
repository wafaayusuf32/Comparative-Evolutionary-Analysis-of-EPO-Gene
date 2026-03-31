# Phase 1: Pairwise Sequence Alignment (DNA Level)

In this first phase, we compared the genomic DNA sequences of the **Human** and **Mouse** EPO gene. Pairwise alignment allows us to understand the direct evolutionary relationship and structural conservation between these two species. We applied both **Global** and **Local** alignment methods to get a complete picture.

---

## 1.1 Global Alignment

**Objective:** To compare the full length of both sequences from end to end to understand the overall structural similarity and gene architecture.

### Methodology
* **Tool:** EMBOSS Needle.
* **Algorithm:** Needleman-Wunsch.
* **Data Source:** NCBI (Genomic FASTA).

### Results
* **Length:** 3880 bp
* **Identity:** 1687/3880 (**43.5%**)
* **Similarity:** 1687/3880 (**43.5%**)
* **Gaps:** 1730/3880 (**44.6%**)

### Biological Interpretation
* **Genomic Divergence:** The 43.5% identity reflects the natural evolutionary distance between humans and mice at the full genomic level.
* **Introns vs. Exons:** The low overall identity is mainly due to the presence of introns (non-coding regions), which accumulate mutations much faster than protein-coding regions.
* **Structural Differences:** The high percentage of gaps (44.6%) indicates that the gene's "architecture" (size and non-coding intervals) has changed significantly, even though the biological function is maintained.

---

## 1.2 Local Alignment

**Objective:** To identify the most highly conserved regions ("islands of similarity") between the two genes, ignoring the highly divergent non-coding stretches.

### Methodology
* **Tool:** EMBOSS Water.
* **Algorithm:** Smith-Waterman.
* **Data Source:** NCBI (Genomic FASTA).

### Results
* **Length:** 3408 bp
* **Identity:** 1685/3408 (**49.4%**)
* **Similarity:** 1685/3408 (**49.4%**)
* **Gaps:** 1261/3408 (**37.0%**)
* **Score:** 4189.0

### Biological Interpretation
* **Isolation of Functional Cores:** The jump in identity (from 43.5% to 49.4%) proves that the local alignment successfully isolated the functional core of the gene, filtering out the most divergent intronic areas.
* **Exon Conservation:** The alignment highlights specific high-matching segments. These segments represent the coding exons that are strictly preserved by natural selection to maintain the proper function of the Erythropoietin protein.
* **Evolutionary Pressure:** The presence of these highly conserved local pockets, despite the overall low global score, indicates strong **negative selection**—where mutations in these vital areas are eliminated to keep the organism viable.
