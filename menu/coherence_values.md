---
layout: page
title: "Mutual Coherence"
author: "Gregor Betz"
---

<!--
  This chapter on mutual coherence is part of the OPMAP-ZKM documentation
  Gregor Betz
-->


<!--OpMAP visualizes multiple opinions as a geographic map. A location in this map represents a particular opinion, and the distance between two locations signifies the extent to which the corresponding opinions cohere with each other. The closer two opinion points in the map, the better they fit together.-->

This document describes how we calculate the degree of mutual coherence between two arbitrary opinions.
<!-- ## Opinions as Sets of Sentences -->

Let's assume Ann and Bob have completed the survey. Their opinions can be represented as sets of sentences. We also assume that all sentences which figure in the debate, and hence in the survey, are numbered. If Ann did for example deny sentence number 8 and accept sentence number 12, her opinion would be `{!8, 12}`, assuming that she suspends judgment with respect to all other sentences.

Let $$A$$ be the set of sentences which represents Ann's opinion, and $$B$$ the set of the sentences which represents Bob's opinion.


## Mutual Coherence as Mutual Support

The opinions represented by $$A$$ and $$B$$ can cohere with each other to different degrees. They maximally cohere if the positions are (logically) equivalent, that is, roughly, if Ann and Bob have essentially the same opinion, except that they may express them in different ways. The opinions don't cohere at all, however, if they are logically inconsistent, i.e., if Ann's and Bob's opinion can't be true in the same time.

The basic idea for measuring mutual coherence between $$A$$ and $$B$$ is to assess how well these opinions support each other: We determine the overall support of $$A$$ by $$B$$ and, vice versa, of $$B$$ by $$A$$, and finally take the mean.

$$Coherence(A,B) = \frac{1}{2} \cdot ( S(A,B) + S(B,A) )$$

The overall support of $$A$$ by $$B$$ is a measure of how the various subsets of $$B$$ support $$A$$. Let $$n\sim B\sim$$ be the number of subsets of $$B$$. We then have

$$S(A,B) = \frac{1}{n\sim B\sim} \cdot \sum{s(A,X)} \text{ for all subsets } X \text{ of } B$$

The problem of computing mutual coherence hence reduces to the calculation of degree of support, s.


## Degree of Support as Degree of Confirmation

The inferential relations between the sentences, encoded in the argument map, decide whether one set of sentences supports or disconfirms another set of sentences. Sentences $$X$$ can support sentences $$Y$$ for quite different reasons:

- $$X$$ contains premisses of arguments whose conclusion is in $$Y$$
- $$X$$ contains premisses of arguments which support arguments whose conclusion is in $$Y$$
- $$X$$ contains sentences which contradict premisses of arguments whose conclusion contradicts $$Y$$
- ...

What we need is a theory that captures all these different cases and allows us, on top, to compute the degree to which one set of sentences supports/disconfirms another one. This theory is provided by a combination of <br>
(i) a model of degrees of justification with<br>
(ii) Bayesian confirmation theory:

1. The degree of justification is a basic measure of how strongly a single sentence is justified in a given debate.
2. Degrees of justification are probabilities.
3. We can hence use probabilistic measures of confirmation and disconfirmation to define the degree of support.
4. Specifically, we use the so-called Kemeny-Oppenheim measure of confirmation as a measure of support $$s$$.

<!--
## Additional Resources

- mutualcoherence.nb -- A Mathematica Notebook which formally defines and applies our measure of mutual coherence.
- mutualcoherence.pdf -- PDF version.
-->
