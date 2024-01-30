# Morphometric analysis of Cannabis leaves (updated)

This repository contains the data and code used in the manuscript Intra-leaf modeling of Cannabis leaflet shape produces leaf models that predict genetic and developmental identities by Balant, M., Garnatje, T., Vitales, D., Hidalgo, O., Chitwood, DH. (Manuscript submitted; currently undergoing journal revisions)

Abstract
The iconic, palmately compound leaves of Cannabis have attracted significant attention in the past. However, investigations into the genetic basis of leaf shape or its connections to phytochemical composition have yielded inconclusive results. This is partly due to prominent changes in leaflet number within a single plant during development, which has so far prevented the proper use of common morphometric techniques.
Here we present a new method that overcomes the challenge of nonhomologous landmarks in palmate, pinnate and lobed leaves, using Cannabis as an example. We model corresponding pseudo-landmarks for each leaflet as angle-radius coordinates and model them as a function of leaflet to create continuous polynomial models, bypassing the problems associated with variable numbers of leaflets between leaves. 
We analyze 341 leaves from 24 individuals from nine Cannabis accessions. Using 3,591 pseudo-landmarks in modeled leaves, we accurately predict accession identity, leaflet number, and relative node number.
Intra-leaf modeling offers a rapid, cost-effective means of identifying Cannabis accessions, making it a valuable tool for future taxonomic studies, cultivar recognition, and possibly chemical content analysis and sex identification, in addition to permitting the morphometric analysis of leaves in any species with variable numbers of leaflets or lobes.

![Alt text](https://github.com/BalantM/Cannabis_leaf_morpho_updated/blob/main/fig_2_new_9_leaflets.jpg)
Figure 1: The process of modeling theoretical leaves for a leaf with (a) three leaflets from accession AM15, (b) five leaflets from accession IKL, (c) seven leaflets from accession FUT75, and (d) nine leaflets from accession IK. The first column shows the scans of the leaves, which we use to extract the outline and place the landmarks on the tip, start, and end of each leaflet and on the petiolar junction (second column). These coordinates are used to generate 200 equidistant pseudo-landmarks on each side of each leaflet, sharing the landmark on the tip of the leaflet for a total of 399 pseudo-landmarks. These coordinates are then converted into polar coordinates. Each transformed leaflet is defined with 399 equidistant pseudo-landmarks, with three landmarks, two at the base and one at the tip. Large points are placed every 25 pseudo-landmarks to emphasize that leaflet outlines are defined by points (third column). Second degree polynomials for angles and for radius from petiolar junction are then fitted through these 399 pseudo-landmarks (fourth column). A modeled theoretical leaf with nine leaflets defined by 3,591 pseudo-landmarks can then be modeled using the collection of 798 polynomial models for each leaf (399 polynomial models for angles and 399 for radius from petiolar junction) (fifth column). 

## Description  
In this repository you can find a dataset composed of 358 leaves from 24 individuals from nine Cannabis accessions, including both wild/feral accessions and cultivated varieties.

- Jupyter notebook 01_trace_leaf.ipynb - extraction of the outlines of the scannes leaves  
- Jupyter notebook 02_model_visualize_leaf_analysis_updated.ipynb - data analysis workflow  
- The folder 03_out containing the files with outline coordinates used in this study  
- The folder 04_land containing the files with landmark corrdinates used in this study  
