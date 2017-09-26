---
layout: page
title: "Methodology"
author: "Tamara Mchedlidze"
---

OpMap is a tool that facilitates sense-making for large-scale debates.

OpMap contains several major components. First a debate is `reconstructed`, i.e. its arguments are analyzed and formalized. An illustrative reconstruction of the veggie-debate is presented [`here`]({{ site.baseurl }}{% link menu/argument_analysis.md %}).

The logical analysis of the debate is used to construct a structured survey. Complex opinion on the debate's topic can be elicited by means of this survey.

The collected opinion data is then translated into a so-called `opinion graph`, the `nodes` of this graph are the opinions held by the participants of the survey, and the weighted `edges` specify how closely related these opinions are. We use [`degree of mutual coherence`]({{ site.baseurl }}{% link menu/coherence_values.md %}) to calculated how related two opinions are.

OpMap then analyzes the resulting weighted graph by applying [`filtering and clustering methods`]({{ site.baseurl }}{% link menu/filtering_clustering.md %}). The static map of the debate is constructed as described [`here`]({{ site.baseurl }}{% link menu/visualization.md %}).

OpMap allows for dynamic updates of the map. Thus, as a new data record is obtained through the survey, the opinion graph, the clustering and the visualization are updated as described [`here`]({{ site.baseurl }}{% link menu/dynamics.md %}).


To summarize, the components of OpMap are:

* [`Debate reconstruction`]({{ site.baseurl }}{% link menu/argument_analysis.md %})

* Opinion elicitation

* [`Computation of the Degree of Mutual Coherence`]({{ site.baseurl }}{% link menu/coherence_values.md %})

* [`Filtering and Clustering`]({{ site.baseurl }}{% link menu/filtering_clustering.md %})

* [`Visualization`]({{ site.baseurl }}{% link menu/visualization.md %})

* [`Dynamics`]({{ site.baseurl }}{% link menu/dynamics.md %})
