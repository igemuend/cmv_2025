# Characterization of human CMV-specific CD8<sup>+</sup> T cells using multi-layer single-cell omics

## Summary
In this study we established a comprehensive workflow to collect multi-omics single-cell data using a commercially available micro-well based platform (BD Rhapsody). This included whole transcriptome, cell surface markers (targeted sequencing-based cell surface proteomics), T cell specificities, adaptive immune receptor repertoire (AIRR) profiles and combinatorial sample multiplexing using two distinct hashing approaches. With this technique we identified paired T cell receptor sequences for three prominent human CMV epitopes. In addition, we review the ability of dCODE dextramers to detect antigen-specific T cells at low frequencies by estimating sensitivities and specificities when used as reagents for single-cell multi-omics.

## Data and Code availability
Human single-cell raw data have been deposited on the European Genome-phenome Archive (EGA) at the accession number EGA50000000594 and are available upon approval by the data access committee (DAC).
This repository contains the original code used to generate the figures presented in the manuscript. To ensure full reproducibility, all analyses were performed in containerized environments using Docker.
- R-based analyses were run using the Docker image `jsschrepping/r_docker:jss_R412_S41` (https://hub.docker.com/r/jsschrepping/r_docker)
- Python-based analyses utilized the Docker image `rnakato/shortcake_light_3.0.0` (https://hub.docker.com/r/rnakato/shortcake_light)

## How to use this repository?
Download all necessary files and scripts from here: https://gitlab.dzne.de/ag-beyer/gemuend_cmv_2025 <br>
To reproduce the figures generated in R, begin with the script `Part1_CMV-Dex_Multiome.Rmd`, which uses the preprocessed Seurat object seurat_filt.h5Seurat. <br>
For the Python-based analyses, continue with the notebook `Part2_CMV-Dex_Multiome.ipynb`. This script can be rerun by loading the files `304_CMV_airr_merged.tsv` and `mudata_fromseurat.h5mu`.

## Publication
Gemünd, I., Bonaguro, L., Becker, M., Müller, S., Joos, C., De Domenico, E., Aschenbrenner, A.C., Schultze, J.L., Moosmann, A., and Beyer, M.D. (2025). Characterization of human CMV-specific CD8+ T cells using multi-layer single-cell omics. Cell Rep. Methods, 101085. 10.1016/j.crmeth.2025.101085. 
The publication can be found under https://doi.org/10.1016/j.crmeth.2025.101085.
