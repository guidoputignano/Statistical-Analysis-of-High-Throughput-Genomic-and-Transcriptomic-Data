# G&T Sequencing

# Table of Contents
1. [Introduction](#introduction)
2. [Technology, Application & Statistics](#technology-application-statistics)
3. [Sources](#sources)
4. [Team members](#team-members)

## Introduction <a name="introduction"></a>
G&T sequencing is a technique for separating and simultaneously obtaining the sequences of genomic DNA and full-length mRNA from single cells, allowing to investigate genetic variation and its effect on gene expression. Isolated single cells are lysed, and polyadenylated RNA is captured using oligo-dT capture primers. RNA is then separated from DNA using streptavidin-coated magnetic beads, after which both are amplified in parallel and sequenced.

![image](https://github.com/AnnaToi01/STA426_main/assets/58418063/27a0dbf3-a622-40dc-b890-b21e14c1b039)
Fig. 1. Technical workflow of G&T-Seq according to Illumina [2].

## Technology, Application & Statistics <a name="technology-application-statistics"></a>

Here is an example of the use of G&T-sequencing data, its application, and the statistical methods used to analyze it.

| Technology                                                                                                                                                                              | Application                                                                                                                                                                                        | Statistics                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                | Source                                                                                                                                                                          |
|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| G&T-seq - simultaneous extraction, amplification, and creation of DNA- and mRNA-seq libraries followed by whole-genome (WGS), whole-exome (WES), and whole-transcriptome sequencing (WTS) | Analysis of genetic diversity and its impact on gene expression. E.g. association of detected copy-number variants (CNVs) and single-nucleotide variants (SNVs) with different expression profiles. | To detect copy number variants (CNV) and single-nucleotide variants (SNV), whole-genome sequencing and whole-exome sequencing were deployed for each cluster's gDNA. As a next step, the CNVs and SNVs were hierarchically clustered with Ward's method (Ward.D2 algorithm, minimizing the sum of squared errors between clusters, unsupervised clustering method) to generate CNV heatmaps and evaluate the clonal architecture of the inferred clusters. Bootstrap was used to infer stable clades and identify different CNV and SNV clones.  Using WTS the relative expression of RefSeq-curated genes was detected.  The single-cell consensus clustering (SC3) approach was chosen for RNA clustering, combining multiple unsupervised clustering methods with a consensus approach.  The heatmaps were used to verify relationships between SNV, CNV, and RNA clones, which are inferred based on the clustering.  | [Genome profiles of pathologist-defined cell clusters by multiregional LCM and G&T-seq in one triple-negative breast cancer patient.](https://doi.org/10.1016/j.xcrm.2021.100404) |


## Sources <a name="sources"></a>
1. [G&T-seq: parallel sequencing of single-cell genomes and transcriptomes by Macaulay *et al.*](https://doi.org/10.1038/nmeth.3370)
2. [G&T-seq by Illumina](https://emea.illumina.com/science/sequencing-method-explorer/kits-and-arrays/g-t-seq.html)
3. [Separation and parallel sequencing of the genomes and transcriptomes of single cells using G&T-seq by Macaulay *et al.*](https://doi.org/10.1038/nprot.2016.138)

## Team Members <a name="team-members"></a>

We are the team *row5right*.

* [AnnaToi01](https://github.com/AnnaToi01)
* [ClaIgl](https://github.com/ClaIgl)
* [LaksL](https://github.com/LaksL)
* [TScholier](https://github.com/TScholier)
