# PET [![travis](https://travis-ci.org/ssadedin/bpipe.svg?branch=master)](https://travis-ci.org/ssadedin/bpipe)

PET: a Pipeline for Enhancer Transcription, a tool for quantify active enhancer RNAs from RNA-seq data

The aim of this project is to quantify transcribed enhancers with a simple command. We will keep on updating it.


## PET online
http://fun-science.club/PET


## Requirements
Bpipe, fastp, STAR, FeatureCounts

    conda install -c bioconda bpipe 
    conda install -c bioconda fastp 
    conda install -c bioconda star 
    conda install -c bioconda subread 
    

## Install
    git clone https://github.com/fun-science-club-ntu/PET


## Usage
    bpipe pipeline.txt rnaseq_1.fastq.gz rnaseq_2.fastq.gz

Index directory of STAR can be changed at the first line pipeline.txt.

This pipeline now supports the Homo sapiens (hg19).


## Input
Fastq files


## Output
Enhancer RNA counts matrix will be in ./count/rnaseq.tab

Quality control and trimmed FASTQ file will be in ./trim/rnaseq.fastq.gz

Aligned BAM file will be in ./mapped/rnaseq.bam


## Downstream analysis
We recommand GREAT (http://great.stanford.edu/public/html/) for functional enrichment analysis and Deseq2 (https://bioconductor.org/packages/release/bioc/html/DESeq2.html) for differential expression analysis.


## Citation
Yingcheng Wu, et al. Multi-omics analysis reveals the functional transcription and potential translation of enhancers. International journal of cancer. vol. 147,8 (2020): 2210-2224. doi:10.1002/ijc.33132



## Contact
PI: Yihui Fan, MD, PhD

Jiangsu Distinguished Professor

Director and Professor, Department of Pathogenic Biology, School of Medicine, Nantong University, Nantong, Jiangsu, China.


Any technical question please contact wuyc@usa.com (Yingcheng Wu)

Copyright (C) 2019-2021 Fan Lab @ NTU.
