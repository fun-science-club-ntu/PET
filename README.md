# ERA [![travis](https://travis-ci.org/ssadedin/bpipe.svg?branch=master)](https://travis-ci.org/ssadedin/bpipe)

ERA: Enhancer RNA Aligner, a tool for quantify active enhancer RNAs from RNA-seq data

The aim of this project is to quantify transcribed enhancers with a simple command. We will keep on updating it.

## Requirements
Bpipe, fastp, STAR, FeatureCounts

    conda install -c bioconda bpipe 
    conda install -c bioconda fastp 
    conda install -c bioconda star 
    conda install -c bioconda subread 
    

## Install
    git clone https://github.com/wuycbio/ERA.git


## Usage
    bpipe pipeline.txt rnaseq_1.fastq.gz rnaseq_2.fastq.gz

Index directory of STAR can be changed at the first line pipeline.txt.

## Input
Fastq files


## Output
Enhancer RNA counts matrix will be in ./count/rnaseq.tab

Quality control and trimmed FASTQ file will be in ./trim/rnaseq.fastq.gz

Aligned BAM file will be in ./mapped/rnaseq.bam

## Downstream analysis
We recommand GREAT for functional enrichment analysis and Deseq2 for differential expression analysis.


## Contact
Any question please contact wuyc@usa.com (Yingcheng Wu)

Copyright (C) 2019 Fan Lab @ NTU.
