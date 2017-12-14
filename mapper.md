# Written by me


---
layout: page
title: Mapper
---

This is a page for the second assignment for Programming for the Social Sciences.
Mapper is a topological data analysis method. Excluding the mathematics behind it can be summarized in these simple steps:
* A filter function, called lens is applied to the data. These can vary in complexity and range from simply taking only one dimension of the data, e.g. take only the x coordinate from a 3-d dataset, to PCA or Isomaps.
* The output of the filter function is broken into overlapping bins
* For each bin (b_i), the inverse image (f^{-1}(b_i)) is taken and all the points are clustered together. Various clustering methods can be used.
* A graph is produced, where each cluster is represented by a vertex and edges between vertices are drawn if the clusters have points in common.

The resulting graph represents the topological shape of the data under the chosen filter.
You can find a notebook with some examples [here](/mapper1.html).
