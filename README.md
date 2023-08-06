# GeneMutationClassification


## Problem Statement

In this project, I am going to build a machine learning model to classify whether a gene is mutated or not based on its read count. As genes mutate so frequently, some mutations are harmful some are not. As we have many datasets already available about the gene mutations. So if we can detect gene is mutated or not of a patient using machine learning models, we can infer other information about the patient like suggesting a similar type of treatment to other patients who also have the same mutation. 

Using gene expression dataset from RNASeq and mutation status of the gene from mutation analysis, a gene may be classified into mutated or not mutated.


## Dataset Used

I used a dataset from The Cancer Genome Atlas (TCGA), a landmark cancer genomics program, molecularly characterized over 20,000 primary cancer and matched normal samples spanning 33 cancer types. The Cancer Genome Atlas (TCGA) is a comprehensive and coordinated effort to accelerate our understanding of the molecular basis of cancer through the application of genome analysis technologies, including large-scale genome sequencing. 

There are many pipelines that simplify the huge TCGA dataset into many types of analysis. One of the most widely used is from Broad Institute of MIT & Harvard. So I used RNA Sequencing of gene profiles(RNASeq), Mutation Analysis(MutSig2CV) from Broad Institute. MRASeq dataset contains information about normalized gene profile of more than 20,000 genes of 172 sample Ids and Mutation Analysis dataset has whether a gene is mutated or not and type of mutation of more than 300 sample Ids. 

Another dataset I used in this project is Pathway Commons data which uses Biological Pathway Exchange (BioPAX) standard to represent data. I used a dataset from Pathway Commons to shortlist features of a gene. Basically, I extracted information about the binary relation of genes other genes from Pathway Commons. The dataset listed all the genes and their relationships with other genes. This dataset has more than 1.8 million relationships between genes. 

In addition, I chose a type of tumor in our brain called Glioblastoma Multiform(GBM-TP) because this type of cancer has relatively more data than other cancers.

The above maintained datasets can be accessed

- RNASeq of GBM-TP: http://gdac.broadinstitute.org/runs/stddata__2016_01_28/data/GBM/20160128/gdac.broadinstitute.org_GBM.Merge_rnaseqv2__illuminahiseq_rnaseqv2__unc_edu__Level_3__RSEM_genes_normalized__data.Level_3.2016012800.0.0.tar.gz.md5

- Mutation Analysis of GBM-TP: https://gdac.broadinstitute.org/runs/analyses__2016_01_28/reports/cancer/GBM-TP/MutSigNozzleReport2CV/GBM-TP.final_analysis_set.maf

- Pathway Commons: https://www.pathwaycommons.org/archives/PC2/v12/PathwayCommons12.All.hgnc.sif.gz


## Machine Learning Algorithms Used
As the problem is binary classification so I used three types of classification algorithms

### Logistic Regression

### Support Vector Machine(SVM)

### Neural Network
