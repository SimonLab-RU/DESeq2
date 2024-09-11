## Guide for the Differential Expression Analysis of RNAseq data using DESeq2

---

### Developed by:

**David R. Requena Anicama, Ph.D.**

- Author's name: David Requena | [Google Scholar](https://scholar.google.com/citations?user=uI01iS4AAAAJ&hl=en) | [ORCID: 0000-0002-5968-1133](https://orcid.org/0000-0002-5968-1133)

**Daniel F. Guevara Díaz, B.Sc.(s)**

- Author's name: Daniel F. Guevara-Díaz | [Google Scholar](https://scholar.google.com/citations?hl=en&user=tqT7vr8AAAAJ) | [ORCID: 0009-0001-2786-8729](https://orcid.org/0009-0001-2786-8729)

---

### Description

This guide provides a comprehensive methodology for performing Differential Expression Analysis (DEA) to identify genes significantly associated with specific conditions or diseases using RNA-Seq data. The process is streamlined with the use of our custom library, [OmicsKit](https://github.com/BigMindLab/OmicsKit), to automate various steps and optimize the analysis workflow. The steps include:

1. **Set up**
	- Install and/or call the required libraries
	- Include OmicsKit library
	- Manage sample metadata
	- Create the DESeq2 object

2. **Exploring confounders**
	- PCA plot
	- tSNE plot
	- UMAP plot
	- HeatMap of Samples

3. **Data Analysis**
	- Retrieve comparisons
	- Obtain mutually exclusive cases
	- Annotation and output tables
	- Apply detectability filter

4. **Plotting**
	- Histogram of p-values
	- Dispersion Estimates
	- MA Plot
	- Volcano Plot
	- HeatMap Samples vs genes
	- Box-Scatter-Violin (BSV) plots

5. **Pathway Enrichment**
	- Overrepresentation Analysis (ORA) and Gene Set Enrichment (GSE)
	- Manage results from Gene Set Enrichment Analysis (GSEA) results' data frames
	- Create balloon plots and concurrency networks of gene sets/pathways

### Requierements

To run the analysis script, the following input files are required:

1. **Mandatory Files:**
   - A metadata table containing sample information (e.g., case/control status, gender).
   - A table of raw gene counts by sample.

2. **Optional Files:**
   - A table specifying genes to be excluded from the analysis (e.g., ribosomal genes).
   - A table listing genes of interest for creating individual gene-specific plots.
