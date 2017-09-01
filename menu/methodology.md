---
layout: page
title: "Methodology"
author: "Tamara Mchedlidze"
---

OpMap is a tool that facilitates sence-making for large scale debates. 
OpMap contains several major components. First a debate is `reconstructed`, i.e. it is formalized as a questionary. 
An example of reconstruction of veggie-debate is presented [`here`]({{ site.baseurl }}{% link menu/argument_analysis.md %}).
Then the quesionary is used to collect data on a particular topic. 
The collected data is then translated to a so-called `opinion graph`, the `nodes` of this graph are the opinions held by the participants of the questionary, and the weighet `edges` specify how closely related these opinions are. We use [`degree of mutual coherence`]({{ site.baseurl }}{% link menu/coherence_values.md %}) function to calculated how related two opinions are. 
We then analyse the resulting weighted graph by applying [`filtering and clustering methods`]({{ site.baseurl }}{% link menu/filtering_clustering.md %}). The static map of the debate is constructed as described [`here`]({{ site.baseurl }}{% link menu/visualization.md %}). 

OpMap allowes for dynamic updates of the map. Thus, as a new data record is obtained through the questionary, the graph opinion graph, the clustering and the visualization are updated as described [`here`]({{ site.baseurl }}{% link menu/dynamics.md %}).


To summarize the components of OpMap are:
* [`Debate reconstruction`]({{ site.baseurl }}{% link menu/argument_analysis.md %})

* [`Computation of the Degree of Mutual Coherence`]({{ site.baseurl }}{% link menu/coherence_values.md %})

* [`Filtering and Clustering`]({{ site.baseurl }}{% link menu/filtering_clustering.md %})

* [`Visualization`]({{ site.baseurl }}{% link menu/visualization.md %})

* [`Dynamics`]({{ site.baseurl }}{% link menu/dynamics.md %})


