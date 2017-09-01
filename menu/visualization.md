---
layout: page
title: "OpMAP Static Visualization"
author: "Tamara Mchedlidze"
---

## Drawing of the Opinion Graph

Drawing of a graph is basically a graphical representation on the plane where the vertices are drawn as dots and edges as lines, connecting the corresponding vertices. There are many ways to draw a single graph.  In order to obtain graph drawing there is a family of algorithms of great computational beauty, so-called `Force-Directed Algorithms`. They are inspired by the mechanical analogy of a mass-spring system: Vertices in the graph can be imagined as spheres which are connected by springs. 
In accordance with the similarity measure the spheres are either attracted to or repelled from each other, until the system converges to a state of minimal energy. Or respectively, the drawing converges to a state in which the more similar vertices are drawn closer to each other and the more dissimilar vertices are farther apart. 

## Generation of Countries Boundaries

This step actually yields the map. Here we use so-called `Voronoi diagrams`. These diagrams divide the 2D plane into regions based on the distance to points on that plane. In our case, the vertices in the drawing. For each vertex there is a corresponding region consisting of all points closer to that vertex than to any other. Finally, the regions corresponding to nodes of the same cluster are given the same colour and we obtain our countries by merging cells of the same colour.
