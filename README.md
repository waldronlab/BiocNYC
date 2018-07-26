Table of Contents
=================

   * [About BiocNYC](#about-biocnyc)
   * [Meet-ups](#meet-ups)
      * [Workflow for Multi-omics Data Analysis by Levi Waldron](#workflow-for-multi-omics-data-analysis-by-levi-waldron)
      * [ChIPSeqSpike: ChIP-Seq data scaling according to spike-in control by Dr. Nicolas Descoste](#chipseqspike-chip-seq-data-scaling-according-to-spike-in-control-by-dr-nicolas-descoste)
      * [Gene set analysis for RNA-seq and microarray gene expression data by Ludwig Geistlinger](#gene-set-analysis-for-rna-seq-and-microarray-gene-expression-data-by-ludwig-geistlinger)
      * [Analysis of ATAC-seq data in R/Bioconductor by Thomas Carroll](#analysis-of-atac-seq-data-in-rbioconductor-by-thomas-carroll)
      * [Microbiome data analysis by the Waldron lab](#microbiome-data-analysis-by-the-waldron-lab)
      * [RNA-seq differential expression with Bioconductor by Davide Risso](#rna-seq-differential-expression-with-bioconductor-by-davide-risso)
      * [Multi-omics infrastructure and data for R/Bioconductor by Levi Waldron](#multi-omics-infrastructure-and-data-for-rbioconductor-by-levi-waldron)

# About BiocNYC

BiocNYC is a group of people with an interest in R/Bioconductor for genomics, based in New York City. It is currently organized primarily by [Levi Waldron of CUNY SPH](http://waldronlab.com), [Davide Risso](http://vivo.med.cornell.edu/display/cwid-dar2062) of Weill Cornell Medical College, [Archana Iyer](https://www.mskcc.org/research-areas/programs-centers/cancer-systems-immunology/contact-us) of MSKCC, and [Thomas Carroll](https://github.com/ThomasCarroll) of Rockefeller University. See https://www.meetup.com/BiocNYC for more information.

We will attempt to post all materials presented at these meetings, see below for links. It's our intention to post videos as well, although technical issues have gotten in the way of several past meetings.

# Meet-ups

## Workflow for Multi-omics Data Analysis by Levi Waldron

July 20, 2018

* https://www.meetup.com/BiocNYC/events/251719874/
* Materials: https://github.com/waldronlab/MultiAssayExperimentWorkshop

This workshop describes an ecosystem of packages and databases for multi-omics data analysis. This includes: 1) MultiAssayExperiment for the representation of multi-omics experiments, 2) SummarizedExperiment for matrix-like datasets, 3) RaggedExperiment for non matrix-like datasets such as SNPs, different types of somatic variants, and segmented copy number, 4) curatedTCGAData, which provides unrestricted 'omics data with merged clinical, pathological, specimen, and subtype data of TCGA as MultiAssayExperiment objects customizable to contain only what you need, 5) TCGAUtils for simplifying common tasks of working TCGA data such as ID-mapping and specimen-type lookup, and 6) MultiAssayExperimentData, under development to provide other integrated multi-omics cancer data starting with 213 cBioPortal datasets.

## ChIPSeqSpike: ChIP-Seq data scaling according to spike-in control by Dr. Nicolas Descoste

April 19, 2018

* https://github.com/lwaldron/BiocNYC-ChIPSeqSpike
* Materials at https://github.com/descostesn/BiocNYC-ChIPSeqSpike

Chromatin Immuno-Precipitation followed by Sequencing (ChIP-Seq) is used to determine the binding sites of any protein of interest, such as transcription factors or histones with or without a specific modification, at a genome scale. The many steps of the protocol can introduce biases that make ChIP-Seq more qualitative than quantitative. For instance, it was shown that global histone modification differences are not caught by traditional downstream data normalization techniques. A case study reported no differences in histone H3 lysine-27 trimethyl (H3K27me3) upon Ezh2 inhibitor treatment. To tackle this problem, external spike-in control were used to keep track of technical biases between conditions. Exogenous DNA from a different non-closely related species was inserted during the protocol to infer scaling factors that enabled an accurate normalization, thus revealing the inhibitor effect. ChIPSeqSpike offers tools for ChIP-Seq spike-in normalization. Ready to use scaled bigwig files and scaling factors values are obtained as output. ChIPSeqSpike also provides tools for ChIP-Seq spike-in assessment and analysis through a versatile collection of graphical functions. ChIPSeqSpike is newly released in the development version of Bioconductor, with a pre-print available at https://www.biorxiv.org/content/early/2018/02/22/269118.

About the speaker:

This workshop will be led by Dr. Nicolas Descoste, author of the ChIPSeqSpike Bioconductor package. Dr. Descoste earned a PhD in Bioinformatics and Genomics at the Centre d'Immunologie de Marseille-Luminy, France. During his PhD, Dr. Descoste studied fundamental transcriptional processes focusing on RNA Polymerase II c-terminal domain. To better understand the inner workings of the genome in terms of mechanistic expression of genes, he joined Danny Reinberg's research group in 2015 as a postdoctoral fellow at New York University. His research focuses on bioinformatic solutions to the study epigenetic mechanisms and transcriptional regulation.

## Gene set analysis for RNA-seq and microarray gene expression data by Ludwig Geistlinger

March 29, 2018

* https://www.meetup.com/BiocNYC/events/248199742/
* Materials are in this repo: [Rmd](https://github.com/waldronlab/BiocNYC/blob/master/GeneSetAnalysis.Rmd) and [built html](https://github.com/waldronlab/BiocNYC/blob/master/GeneSetAnalysis.html)

Gene set analysis encompasses a broad range of methods differing greatly in objectives and interpretation of results. This workshop will help participants understand the distinctions between assumptions and hypotheses of existing methods for enrichment analysis of gene expression data. It will provide code and hands-on practice of all necessary steps for differential expression analysis, gene set- and network-based enrichment analysis, and identification of enriched genomic regions and regulatory elements, along with visualization and exploration of results.

About the speaker: Dr. Ludwig Geistlinger is a post-doctoral fellow in the Waldron lab, specializing in enrichment methods and analysis.

## Analysis of ATAC-seq data in R/Bioconductor by Thomas Carroll

Feb 16, 2018

* https://www.meetup.com/BiocNYC/events/247121601/
* Materials at https://github.com/ThomasCarroll/ATAC_Workshop

The use of ChIP-seq, DNA-seq and MNAse-seq to identify transcription factor binding, open chromatin and nucleosome positions respectively has led to a broader understanding of epigenetic events across the genome. ATAC-seq (Assay for Transposase Accessible Chromatin with high-throughput sequencing) offers a method to rapidly and simultaneously identify openchromatin, nucleosome positioning and transcription factor binding at a genome scale. In this session, we will review the alignment, pre-processing and peak calling of ATAC-seq data in R/Bioconductor and will perform quality control, identification of replicated peaks, annotation of peaks to genes and visualization of ATAC-seq data in IGV.


## Microbiome data analysis by the Waldron lab

Dec 15, 2017

Audrey Renson, Lucas Schiffer, Levi Waldron

* https://www.meetup.com/BiocNYC/events/243813429/ 
* Materials at https://github.com/waldronlab/MicrobiomeWorkshop/tree/BiocNYC-2017-12-15
* short-cut gists to [install needed packages](https://gist.github.com/lwaldron/220828bae0764a80fcf3a23868bf182e) and [download essential data](https://gist.github.com/lwaldron/c1e44d0516422777e3f87d6726d45332).

Bioconductor provides significant resources for microbiome data acquisition, analysis, and visualization. This workshop introduces the common analyses of differential abundance and ordination using the phyloseq, edgeR, and DESeq2. It will utilize the curatedMetagenomicData package, a resource providing uniformly processed taxonomic and metabolic functional profiles for more than 6,000 whole metagenome shotgun sequencing samples from 26 publicly available studies, including the Human Microbiome Project. At the end of this workshop, users will be able to access publicly available metagenomic data and to perform differential abundance tests, ordination, and visualization of microbiome data in R/Bioconductor.

I will briefly introduce the topic and scope of the workshop, and brief (10-minute) talks by two active microbiome researchers in my lab:

1. Audrey Renson will summarize results from an analysis of sociodemographic patterning of the oral microbiome in the New York City Health and Nutrition Examination Study (NYC-HANES). https://www.biorxiv.org/content/early/2017/10/25/189225
2. Lucas Schiffer will demonstrate the use of curatedMetagenomicData for meta-analysis of health outcomes. Free link to article at Nature Methods: http://rdcu.be/A27v

Then we will supervise a hands-on workshop on analyzing microbiome data in R/Bioconductor. 


## RNA-seq differential expression with Bioconductor by Davide Risso

Oct 27, 2017

* https://www.meetup.com/BiocNYC/events/244210806/
* Materials at: https://github.com/drisso/rnaseq_meetup

In this hands-on workshop I will show you how to perform exploratory data analysis, normalization, and differential expression of RNA-seq data using popular Bioconductor packages, such as edgeR and DESeq2. To get the best out of the workshop, please bring your laptop with the latest version of R and Bioconductor already installed. I will follow up with a list of packages that we will use during the workshop.

About the speaker:

Davide Risso is an Assistant Professor in the Division of Biostatistics and Epidemiology, Department of Healthcare Policy and Research, Weill Cornell Medicine. Prof Risso is author and/or maintainer of six Bioconductor packages for the analysis of (single-cell) RNA-seq data.

## Multi-omics infrastructure and data for R/Bioconductor by Levi Waldron

Sept 29, 2017

* https://www.meetup.com/BiocNYC/events/243180166/
* Materials at: https://www.slideshare.net/LeviWaldron/multiomics-infrastructure-and-data-for-rbioconductor/1

Multi-omics experiments are increasingly commonplace in biomedical research, and add layers of complexity to experimental design, data integration, and analysis. R and Bioconductor provide a generic framework for statistical analysis and visualization, as well as specialized data classes for a variety of high-throughput data types, but methods are lacking for integrative analysis of multi-omics experiments. This talk introduces the recent MultiAssayExperiment class and methods, with integrated datasets and analyses of The Cancer Genome Atlas. It also introduces curatedMetagenomicData, a curated resource of taxonomic, gene, and metabolic functional profiles for thousands of human microbiome samples.
