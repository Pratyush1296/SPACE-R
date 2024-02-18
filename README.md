# SPACE-R
This repository has been provided for the creation of citation networks and generating recommendations for a given input paper. The current version has four different datasets corresponding to two fields namely "Information Systems" and "Physics" downloaded from ArnetMiner (https://aminer.org/aminernetwork) and Web of Science Core Collection (http://www.webofknowledge.com/WOS). 

Each dataset has the following files:\
a) paper_info.csv - the list of papers and their associated metadata like title, abstract, authors, publication venues etc. \
b) original factors.csv - This file contains certain paper-related, author-related and journal-related factors which have an impact on the citation counts of a paper have also been provided. \
c) new_factors.csv - This file contains the latest set of factors that have been used for the SPACE-R algorithm
d) citation_edges_unweighted.csv - The edgelist for creating an unweighted citation network
e) cite_edges.csv - The edgelist that includes the citation relationship, the popularity index scores for source and target nodes, and the corresponding edgeweights for the creation of a weighted directed network. The popularity score index has been generated using PCA from the factors influencing citation counts.  
f) Modularity.csv (optional) - The community distribution of all papers based on the weighted citation network

While most of the factors have been generated and the results are included as data files, in order to generate the factors for yourself, additional data has been provided in the respective dataset folders. These files include the necessary information for generating the factors used in PCA. The code for computing the factors has also been provided under the codes folder. For the AMiner dataset, the data can be accessed here: https://drive.google.com/drive/folders/1Kv39_6KsGXSVrQ940Y0vvIGNTaWPOyQv?usp=drive_link

For WoS dataset, additional pre-processing is required to generate the factors especially for authors. The author disambiguation strategy used for the same has been provided under the codes repository for this purpose. 

# Dataset Statistics

The total number of papers, authors and the citation relationships for each dataset have been summarized in the table below. In addition, the degree values for each network are also recorded. 

|Dataset         |No of Papers|No of Authors|No of Citation Relationships|Degree    |
|----------------|------------|-------------|----------------------------|----------|
|IS (AMiner)     |    31225   |49783        |   76458                    |4.898     |
|Physics (AMiner)|    10669   |21590        |   32368                    |6.068     |
|IS (WoS)        |    46502   |57765        |  126843                    |5.456     |
|Physics (WoS)   |    29601   |49605        |   96609                    |6.521     |
