# SPACE-R
This repository has been provided for the creation of citation networks and generating recommendations for a given input paper. The current version has four different datasets corresponding to two fields namely "Information Systems" and "Physics" downloaded from ArnetMiner (https://aminer.org/aminernetwork) and Web of Science Core Collection (http://www.webofknowledge.com/WOS). 

Each dataset has the following 3 files:\
a) paper_info.csv - the list of papers and their associated metadata like title, abstract, authors, publication venues etc. \
b) factors.csv - This file contains certain paper-related, author-related and journal-related factors which have an impact on the citation counts of a paper have also been provided. \
c) citation_edges.csv - The edgelist for which includes the citation relationship, the popularity index scores for source and target nodes, and the corresponding edgeweights for the creation of a weighted directed network. The popularity score index has been generated using PCA from the factors influencing citation counts. 

# Dataset Description

