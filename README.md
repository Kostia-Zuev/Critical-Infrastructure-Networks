# Critical Infrastructure Networks 
Network data repository

[![DOI](https://zenodo.org/badge/87771758.svg)](https://zenodo.org/badge/latestdoi/87771758)


### Power Grids

#### 1. US Power Grid

- Filename: 'uspowergrid.mat'

- Format: edge list represented by m-by-2 matrix, each row [i,j] represents a link between nodes i and j. 

- Size: n=4941 nodes, m=6594 links

- Description: 
An undirected, unweighted network representing the topology of the Western States Power Grid of the United States. 
Nodes represent transformers, substations, and generators. Links represent high-voltage transmission lines.

- Remark: 
The transmission lines can be directed and weighted (differentiated based on their capacity), but this information is not available.

- Data Source: 
Originally compiled by D. Watts and S. Strogatz and used in 
D.J. Watts and  S.H. Strogatz (1998) "Collective dynamics of “small-world” networks," Nature 393, 440-442.
Availalbe online at: https://toreopsahl.com/datasets/#uspowergrid
