# Critical Infrastructure Networks 
Network data repository

[![DOI](https://zenodo.org/badge/87771758.svg)](https://zenodo.org/badge/latestdoi/87771758)

## Citing CIN repository
If you find this network data collection useful in your work, I encourage you to cite the repository. 
You can use the following BibTeX citation:

```
@misc{KZ_CIN_2017_545662,
  author       = {Konstantin M. Zuev},
  title        = {Kostia-Zuev/Critical-Infrastructure-Networks v1.0},
  month        = apr,
  year         = 2017,
  doi          = {10.5281/zenodo.545662},
  url          = {https://doi.org/10.5281/zenodo.545662}
}
```

## Data Format
Each network is available in three different formats: `.mat`, `.cvs`, and `.txt`.
* `.mat` file contains at least three variables:
  - A is a sparse n-by-n [adjacency matrix](https://en.wikipedia.org/wiki/Adjacency_matrix), where n is the number of nodes (vertices). If a network is undirected and unweighted, then A is symmetric, A(i,j)=1 if there is a link (edge) between nodes i and j, and A(i,j)=0 otherwise. If a network is directed, then A is not necessarily symmetric and A(i,j)=1 if there is a link from i to j (and zero otherwise). If a network is weighted, then A(i,j) is the weight of the link from i to j (a zero weight means no link).  
  - L is an edge list. If a network is undirected and unweighted, then L is m-by-2, where m is the number of links and a row [i,j] represents a link between nodes i and j. If a network is directed, then a row [i,j] represents a link from i to j. If a network is weighted, then L is m-by-3, where the 3rd column contains weights. 
  - G is a [MATLAB graph object](https://www.mathworks.com/help/matlab/graph-and-network-algorithms.html) representing the network. 
* `.cvs` and `.txt` files contain an edge list, which is the same as L above.

## Power Grids

### 1. Western States Power Grid of the United States

- Path: [Critical-Infrastructure-Networks/power-grids/us-western-states/](https://github.com/Kostia-Zuev/Critical-Infrastructure-Networks/tree/master/power-grids/us-western-states)
   
* Description: 
An undirected, unweighted network representing the topology of the Western States Power Grid of the United States. 
Nodes represent transformers, substations, and generators. Links represent high-voltage transmission lines.

* Remark: 
The transmission lines can be directed and weighted (where weight describe their capacity), but this information is not available.

* Data Source: 
Originally compiled by D. Watts and S. Strogatz and used in 
D.J. Watts and  S.H. Strogatz (1998) "Collective dynamics of “small-world” networks," Nature 393, 440-442.
Availalbe online at: https://toreopsahl.com/datasets/#uspowergrid

* Basic [Network Properties](https://en.wikipedia.org/wiki/Network_science#Network_properties)

Property | Value
-------- | -------------
Number of nodes | 4941
Number of links  | 6594
Density | 5.403e-04
Maximum degree | 19
Average degree | 2.669
Average clustering coefficient | 0.106
Number of connected components | 1
Diameter  | 46 
Average shortest path length | 18.989


![alt tag](https://github.com/Kostia-Zuev/Critical-Infrastructure-Networks/blob/master/power-grids/us-western-states/powergridUSWS.png)
