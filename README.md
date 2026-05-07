# Variant-Analysis-and-Transcriptomics-Pipeline

## Overview
This project demonstrates an end-to-end bioinfromatics workflow for next-generation sequencing (NGS) variant analysis and functional annotation using industry standard tools including:

- FastQC
- MultiQC
- BWA
- SAMtools
- bcftools
- Ensemble VEP

The pipeline performs:
- sequencing quality control
- read alignment
- BAM processing
- variant calling 
- functional annotation
- biological interpretation of genomic variants

---

## Objectives

- Perform quality assessment of raw FASTQ sequencing reads
- Align sequencing reads to the GRCh38 human reference genome
- Process and index BAM alignment files
- Identify genomic variants using bcftools
- Annotate variants using Ensembl Variant Effect Predictor (VEP)
- Interpret functional consequences of genomic variants

---

## Tools & Technologies
| Tool | Purpose |
|---|---|
| FastQC | Sequencing quality control |
| MultiQC | Aggregated QC reporting |
| BWA | Read alignment |
| SAMtools | BAM processing |
| bcftools | Variant calling |
| Ensembl VEP | Functional annotation |
| Linux / Bash | Pipeline execution |
| Git & Github | Version control |

---

## Workflow
'''text
FASTQ Files
↓
Quality Control (FastQC / MultiQC)
↓
Read Alignment (BWA)
↓
BAM Sorting & Indexing (SAMtools)
↓
Variant Calling (bcftools)
↓
Variant Annotation (Ensembl VEP)
↓
Biological Interpretation
'''

---

## Project Structure

```text
Variant-Analysis-and-Transcriptomics-Pipeline/
│
├── data/
│ ├── raw/
│ ├── processed/
│ └── reference/
│
├── results/
│ ├── qc/
│ ├── bam/
│ └── variants/
│
├── scripts/
├── notebooks/
├── docs/
└── README.md
```

---

## Variant Annotation Results

Variant annotation was performed using Ensembl VEP against the GRCh38 reference genome

Generated outputs include:

- 'interpretable_variants.txt'
- 'high_impact.txt'
- 'moderate_impact.txt'
- 'variant.vep.vcf'
- 'variant.vep.vcf_summary.html'

---

## Biological Interpretation

Most detected variants were classified as:

- intron variants
- upstrewam gene variants
- splice-associated variants

The majority of variants were categorized as MODIFIER impact variants, which is expected because many genomic variants occur outside protein-coding exons.

Annotated genes identifies in the analysis included:

- PRDM16
- CHD5
- EPHA2
- PEX14
- RERE

These genes are associated with transcriptional regulation, signaling pathways, chromatin organization, intercellular transport.

A subset of varinats affected splice-associated regions, which may influence RNA splicing and transcript processing.

---

## Skills Demonstated
- End-to-end NGS analysis
- Linux command-line bioinformatics workflows
- Variant calling and annotation
- Functional interpretation of genomic variants
- Reproducible pipeline development
- Data organization and workflow management
- Git/Github version control
- Biological data interpretation

---

## Future Improvements 

- Integration with ClinVar and gnomAD databases
- RNA-seq differential expression
- Visualization dashboards
- Automated workflow scripting
- Machine learning-based variant prioritization

---

## Author

Annie Sugandha Parimala Telagathoti
M.S. Biology | Bioinformatics & Genomics Enthusiast
