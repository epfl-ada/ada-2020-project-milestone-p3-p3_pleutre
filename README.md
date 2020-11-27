Products clusters and interactive  visualization
======

## Abstract
While the paper establishes the validity of the Tesco 1.0 dataset we propose to use this dataset to study if we can find some similarity in the typical products consumed within geographically close areas. To do so we will study the clusters of areas computed out of their products consumption : areas with similar typical products consumption will be clustered together. And then we will compare these clusters with the geographic disposition of the areas. Such a clustering could help grocery shop compagnies to adapt their product according to the areas where they operate. Moreover, to provide a better understanding of the data we will create an interactive visualization. The latter will represent typical food consumption of London areas on a map of the city with different levels of aggregation, over different periods of time and with the possibility of choosing different attributes of the typical product. This visualisation will help assess the validity of our findings.

## Research questions

1. Are similar areas in terms of typical products geographically close?
2. Can we naturally cluster areas geographically when it comes to food consumption in London?
3. How do those clusters differ when we vary the aggregation level?
4. In the context of an advertising campaign, which areas of the city should be associated with which kind of products? 

## Proposed datasets

1. “Tesco grocery 1.0” -- This dataset contains all the necessary information to create the clusters described above.
2. “Statistical GIS Boundary Files for London” -- This dataset will help us to relate the areas of the Tesco dataset with their real geographical positions, needed for the visualization.

## Methods :

For the visualization task, we will use the library geopandas. In this visualization we will include a scrollbar linked to the time (month) variable of the represented data. We will also add some checkboxes to change the aggregation (ward,lsoa,msoa) level of the represented data. 
For the clustering part, we will cluster the areas according to the product consumption of their products using the two following methods:
1. Apply the k means algorithm on the data (need also to find suitable k)
2. Produce a proximity graph with vertices being the areas and edges representing the similarity between them. We will then compare the value of these edges with the geographical distance between the areas (vertices).

## Proposed timeline :

We intend to work simultaneously on both of the tasks. For the clustering part we will first work the k means method, then on the proximity graph and finally we will compare the results with the geographical positions of the areas. Of course, the finishing touches of the visualization will need the results of the clustering part, so it will be finished last.

## Organization within the team :
Since we think that the visualization is the easiest part we will distribute the tasks as follows:

* clustering: Lucas Giordano and Augustin
* visualization: Lucas Gruaz

We will of course work together and help each other to overcome any issues encountered, but this shows what we will be most focused on.
