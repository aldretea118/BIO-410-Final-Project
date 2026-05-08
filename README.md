# BIO-410-Final-Project
## Background
This data consist of 6 samples from the organism Zaire Ebola Virus. This organism is a prokaryote which is transmitted through humans and mammals.
# Citation 
  Grard G, Biek R, Tamfum JJ, Fair J, Wolfe N, Formenty P, Paweska J, Leroy E. Emergence of divergent Zaire Ebola Virus strains in Democratic Republic of the Congo in 2007 and 2008. J Infect Dis. 2011 Nov;204 Suppl 3(Suppl 3):S776-84. doi: 10.1093/infdis/jir364. PMID: 21987750; PMCID: PMC3218671.

## Purpose
The purpose of this project was to create a phylogenic tree from 6 samples of zaire ebolavirus in order to determine the evolutionary relationships between the samples. 

## Methods
- Sequencing reads (NGS next-generation sequencing)
    >We sequenced 6 samples of [Zaire Ebola Virus](
    
- Assembly using [MEGAHIT](https://github.com/voutcn/MEGAHIT)
    > In terminal the following code was run to utilized in terminal:
      >conda install -c bioconda megahit
      >megahit -1 sim_t1_1.fq -2 sim_t1_2.fq -o t1_out (changing t1 for each sample through 6) 
    >(https://www.anaconda.com/docs/getting-started/miniconda/install/mac-cli-install)

- Alighment using a package DECIPHER
    >We aligned the raw data in folder sequences in R studio using package DECIPHER

- Tree using ML method in a package DECIPHER
    >We created a phylogenetic tree using the DECIPHER package with the following code in R studio:
    >tree <- Treeline(alignment, method = “ML”, showplot = TRUE)
    
- The assembled reads are in t<#>_out directories and the raw sequencing reads are in [Andrea](https://github.com/aldretea118/BIO-410-Final-Project/tree/main/andrea)
  

## Results

Here is phylogenetic tree
[Phylogenetic Tree](https://github.com/aldretea118/BIO-410-Final-Project/blob/main/Phylogenetic%20Tree.pdf)

Explain
- From the phylogenetic tree, it appears that the samples that were most closely related to each other were:
    > 3 & 10, 4 & 11, 9 & 12, 7 & 14, 5 & 12, 13 & 6, and lastly 8 & 1. 
- How many individuals did these 6 samples come from (probably) based on the phylogenetic tree 
