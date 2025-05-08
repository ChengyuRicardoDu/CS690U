# CS690U Final Project
## Overview
Clustering biological sequences can help reveal functional or evolutionary relationships without the need for labeled data.
In this project, we evaluated how well simple k-mer frequency features, combined with classical clustering algorithms,
can recover known biological classes in two sequence datasets: E. coli noncoding RNAs and MopB family proteins. For
RNA, where classes are defined by short, conserved motifs, k-mer clustering performed remarkably well—surpassing most
foundation models. In contrast, for the MopB protein dataset, where functional signals are more subtle and distributed,
foundation models clearly outperformed k-mers. We also observed that mid-layer embeddings from foundation models
sometimes yielded better clustering than final layers, likely due to better retention of motif-level details. These findings
highlight both the power and limitations of simple sequence features, and suggest that the choice of models should be guided
by the biological structure of the data.


## Repository Structure

├── README.md

├── K-mer Test.ipynb # Jupyter Notebook for analysis

├── Plots.rmd # R Markdown script to generate plots

├── ecoli_vmeasure.png # V-measure plot for RNA dataset

├── mopb_vmeasure.png # V-measure plot for protein dataset
