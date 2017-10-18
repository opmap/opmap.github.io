---
layout: page
title: "Methodology"
author: "Tamara Mchedlidze"
---

OpMAP is a tool that facilitates sense-making for large-scale debates. It contains several major components.

* First, the debate is *reconstructed*, i.e. its arguments are analyzed and formalized. An illustrative reconstruction of the Veggie-debate is presented [here]({{ site.baseurl }}{% link menu/argument_analysis.md %}).

* Second, the logical analysis of the debate is used to construct a structured [survey]({{ site.baseurl }}{% link menu/survey.md %}). Complex opinions on the debate's topic can be elicited by means of this survey.

* Third, the collected opinion data is translated into a so-called [opinion graph]({{ site.baseurl }}{% link menu/opinion_graph.md %}). The *nodes* of this graph are the opinions held by the participants of the survey, and the *weighted edges* specify how closely related these opinions are. We use [degree of mutual coherence]({{ site.baseurl }}{% link menu/coherence_values.md %}) to calculate how related two opinions are.

* Then, the resulting weighted graph is analyzed by applying [clustering and filtering methods]({{ site.baseurl }}{% link menu/filtering_clustering.md %}). 

* The initial map of the debate is then constructed as described [here]({{ site.baseurl }}{% link menu/visualization.md %}).

* Finally, OpMAP allows for dynamic updates of the map: As a new data record is obtained through the survey, the opinion graph, the clustering and the visualization are updated as described [here]({{ site.baseurl }}{% link menu/dynamics.md %}).


To summarize, the steps to generate a dynamic opinion map are:

* [1. Debate reconstruction]({{ site.baseurl }}{% link menu/argument_analysis.md %})

* [2. Obtaining an opinion sample]({{ site.baseurl }}{% link menu/survey.md %})

* [3. Creating a graph from the opinion sample]({{ site.baseurl }}{% link menu/opinion_graph.md %})

* [4. Computation of the Degree of Mutual Coherence]({{ site.baseurl }}{% link menu/coherence_values.md %})

* [5. Filtering and clustering]({{ site.baseurl }}{% link menu/filtering_clustering.md %})

* [6. Visualization]({{ site.baseurl }}{% link menu/visualization.md %})

* [7. Adding dynamics]({{ site.baseurl }}{% link menu/dynamics.md %})
 