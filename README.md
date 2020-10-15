# Epigenomic characterisation of the giant cell tumor of bone


This repository contains source code behind this preprint:

https://www.medrxiv.org/content/10.1101/2020.05.26.20089888v1


## Essential steps of the GCTB analysis

1. Initial processing of the whole-genome sequencing data, including SNP and CNV calling, was performed with the DKFZ/PCAWG WGS analysis workflow, available as a Docker container from: 

https://dockstore.org/containers/quay.io/pancancer/pcawg-dkfz-workflow

Structural variant identification with SOPHIA:

https://bitbucket.org/utoprak/sophia/src

2. A compatible CWL worfklow for the intial processing ot the whole-genome bisulfite data, from reads to methylation calls:

https://github.com/CompEpigen/WGBS_workflows/CWL/workflows/BWA_meth_start_with_trimmed.cwl

3. A compatible CWL workflow for ATAC-seq data, from reads to genome signal tracks, is available from:

https://github.com/CompEpigen/ATACseq_workflows

4. A compatible CWL workflow for ChIPmentation data, from reads to genome signal tracks:

https://github.com/CompEpigen/ChIPseq_workflows

5. A snakemake-based processing workflow for RNA-seq data:

https://github.com/CompEpigen/RNASeq_GCTB. 

6. Code for calling of LMDs from WGBS data:

https://github.com/lutsik/CP-LMDs






