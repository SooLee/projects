# projects

* [4DN DCIC Pipelines](#4dn-dcic-pipelines)
* [Pairix](#pairix)
* [Older projects](#older-projects)
    * [EMSAR](#emsar)
    * [Alignment-free module for NGSCheckmate](#alignment-free-module-for-ngscheckmate)
* [Keywords](#keywords)

## 4DN DCIC pipelines
* The pipelines are for automatic and unified data processing for [4DNucleome](#4dnucleome).
* The pipelines are set up on [Amazon Web Service](#amazon-web-service).
* The components are encapsulated in [docker](#docker) containers.
* The pipelines are described using [Common Workflow Language](#common-workflow-language).
* The pipelines are triggered and managed using [Lambda](#lambda) and [APIGateway](#apigateway), which are combined using [Chalice](#chalice).
* The pipelines are run on the [Seven Bridges](#seven-bridges) platform.

## Pairix
* https://github.com/4dn-dcic/pairix
* Pairix is an extension from [tabix](#tabix) for 2D indexing and querying.
* Pairix works on text files compressed using [bgzip](#bgzip).
* Pairix is written in [C](#c).
* Pairix has a companion python module, pypairix, based on [Python C extension](#python-c-extension).
* Pairix can be used for querying specific genomic ranges for analyzing [Hi-C](#hi-c) data.

## Older projects
### EMSAR
* https://github.com/parklab/emsar
* EMSAR is a tool for quantifying transcript isoform abundance from [RNA-seq](#rna-seq) data.
* EMSAR is written in [C](#c).
* EMSAR uses a modified [suffix array](#suffix-array) data structure for creating an index of shared k-mers or paired k-mers among transcripts (k=read length)
* EMSAR uses [Maximum likelihood estimation](#maximum-likelihood-estimation) on joint [Poisson distribution](#poisson-distribution), whose expected values are represented by the sum of abundance parameters to estimate.
* EMSAR reads alignment files in [BAM](#bam) or SAM format using [samtools C library](#samtools-c-library).

### Alignment-free module for NGSCheckmate
* https://github.com/parklab/ngscheckmate
* NGSCheckmate is a tool for detecting sample swaps among genomic data in FASTQ, BAM and VCF formats.
* The Alignment-free module for NGSCheckmate detects sample swaps in [FASTQ](#fastq) files.
* The Alignment-free module for NGSCheckmate creates and uses a [hash](#hash) table for k-mers spanning a selected set of [single nucleotide polymorphisms (SNPs)](#single-nucleotide-polymorphism) to quantify allelic fraction.
* The Alignment-free module for NGSCheckmate is written in [C](#c)


## Keywords
* 4DNucleome
* Amazon Web Service
* Docker
* Common Workflow Language
* Lambda
* APIGateway
* Chalice
* Seven Bridges
* tabix
* C
* Python C extension
* bgzip
* Hi-C
* RNA-seq
* Suffix array
* Maximum likelihood estimation
* Poisson distribution
* BAM
* Samtools C library
* FASTQ
* Single nucleotide polymorphism
