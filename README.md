# Centenarian SNP Analysis

This repository contains R scripts used to identify, filter, and compare single nucleotide polymorphisms (SNPs) in centenarian and supercentenarian genome data.

## Files Included

- **snp_analysis_supercentenarian** – Main R script to:
  - Read VCF files and extract mutations.
  - Filter variants based on quality (PASS).
  - Sort SNPs from different individuals.
  - Identify unique and common SNPs among supercentenarians.

## Overview of Workflow

1. **VCF Parsing**: Reads the `.vcf` file and extracts all mutations from `chr1`.
2. **Filtering**: Keeps only `PASS` mutations for downstream analysis.
3. **SNP Sorting**: Organizes SNP positions from multiple individuals.
4. **Uniqueness Detection**: Finds SNPs unique to individuals or shared among supercentenarians.

## Requirements

Install the required R packages before running the script:

```R
install.packages("vcfR")
install.packages("openxlsx")
install.packages("readxl")
