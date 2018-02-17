Table of Contents
=================

   * [About BiocNYC](#about-biocnyc)
   * [Meet-ups](#meet-ups)
      * [Analysis of ATAC-seq data in R/Bioconductor by Thomas Carroll](#analysis-of-atac-seq-data-in-rbioconductor-by-thomas-carroll)
      * [Microbiome data analysis by the Waldron lab](#microbiome-data-analysis-by-the-waldron-lab)
      * [RNA-seq differential expression with Bioconductor by Davide Risso](#rna-seq-differential-expression-with-bioconductor-by-davide-risso)
      * [Multi-omics infrastructure and data for R/Bioconductor by Levi Waldron](#multi-omics-infrastructure-and-data-for-rbioconductor-by-levi-waldron)

# About BiocNYC

BiocNYC is a group of people with an interest in R/Bioconductor for genomics, based in New York City. It is currently organized primarily by [Levi Waldron of CUNY SPH](http://waldronlab.com), [Davide Risso](http://vivo.med.cornell.edu/display/cwid-dar2062) of Weill Cornell Medical College, [Archana Iyer](https://www.mskcc.org/research-areas/programs-centers/cancer-systems-immunology/contact-us) of MSKCC, and [Thomas Carroll](https://github.com/ThomasCarroll) of Rockefeller University. See https://www.meetup.com/BiocNYC for more information.

We will attempt to post all materials presented at these meetings, see below for links. It's our intention to post videos as well, although technical issues have gotten in the way of several past meetings.

# Meet-ups

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
