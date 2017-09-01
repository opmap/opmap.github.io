---
layout: page
title: Argument Analysis
---

<!--
 This chapter on argument analysis is part of the OPMAP-ZKM documentation
 Gregor Betz
 -->


# Argument Analysis

The OPMAP installation is based on an argumentative analysis of the Veggie Debate. By completing [the survey](/link_to_survey_chapter), you actually judge different arguments that have been advanced in the debate. The argumentative analysis is later used to [compute the degree](/link_to_coherence_chapter) to which your opinion coheres with the opinions of other users.

This document introduces the argumentative analysis of the Veggie Debate and the technical tools we've employed to carry it out.

## The Main Theses of the Veggie Debate

In our interpretation, the Veggie Debate is essentially a debate about the following core claims: 

```
[Meat-OK]: There exist meat and animal products 
which one is allowed to eat.

[Eat-what-you-want]: One may eat meat and other 
animal products of any kind.

[No-mass-farming]: One must not eat meat produced 
in modern mass farming facilities.

[Strict-veggie]: One must not eat meat at all.

[Strict-vegan]: One must not eat animal products 
at all.

[Less-meat]: One should reduce the consumption 
of meat.

[Less-animal]: One should reduce the consumption
of animal products.
```

These claims are related in different ways. For example, `[Eat-what-you-want]` contradicts `[No-mass-farming]`, that is, you cannot maintain both claims in a self-consistent way. Or, `[Strict-vegan]` implies `[Strict-veggie]`, that is, if you accept the former, you inevitably accept the latter claim, too.

The different logical relations between the core claims are encoded in our argumentative analysis.


## The Veggie Debate Argument Map

The argumentative analysis first and foremost clarifies the various pros and cons of the Veggie Debate. These pro and con reasons are reconstructed as arguments for or against the different core claims of the debate. 

We distinguish the following kinds of arguments:

- Culinary Considerations
- Health Considerations
- Financial Considerations
- Naturalness and Normality Considerations
- Climate Change Considerations
- Arguments from Nature Conservation  
- Animal Rights Arguments
- World Nutrition Considerations
- Arguments from Personal Autonomy

These categories are used to group the different arguments. The following *argument map* provides an overview of all the arguments of the debate. 

<!--Maybe we use a slide show, here, or an animated GIF?-->
![Veggie Debate Argument Map](images/veggie_debate.pdf)

The red and green arrows indicate relations of support and attack between the various arguments and theses. Further information on how to read an argument map can be found [here](http://www.argunet.org/2013/04/03/so-what-exactly-is-an-argument-map/).


## Having a Closer Look at an Argument

Every argument of the debate is reconstructed as a series of *premisses* that justify a *conclusion*.

Premisses
:	= the statements which an argument takes for granted and which are used to justify the conclusion.

Conclusion
:	= the statement an argument is supposed to back up, or justify.

So, for example, the argument for `[No-mass-farming]` which stresses the suffering of animals in mass-farming facilities is analysed as:

```
<Animal suffering>: Animal rights are flagrantly 
violated in modern mass-farming facilities.

(1) Animal rights are flagrantly violated in modern 
mass-farming facilities.
(2) By eating food that has been produced in conventional 
ways, esp. through mass-farming techniques, one 
supports the modern mass-farming industry.
(3) One must not support an industry which is responsible
for systematic violations of animal rights.
----
(4) [No mass farming]: One must not eat meat produced 
in modern mass farming facilities.
```

Here, `(1)`-`(3)` serve as premisses of the argument `<Animal suffering>` with conclusion `(4)`.

The different considerations of the debate are reconstructed as *valid* arguments. Valid arguments are "complete" in the following sense: If one accepts all premisses, one has to accept the conclusion. We say: the arguments define inferential relations between the various statement which figure in the debate.

(Who "forces" you to accept the conclusion if you accept the premisses? That's our language. For example, you cannot consistently say both that 'Ann is ill *and* Bob is ill' and that 'Bob is *not* ill' -- unless you use the words "and" or "not" in a very different way than we usually do.)



## Argdown -- Our Argument Mapping Technology

We're using the newly developed Argdown Technology to carry out the argumentative analysis.

- http://christianvoigt.github.io/argdown/
- https://github.com/christianvoigt/argdown/

Argdown is basically a syntax, i.e., a set of conventions for structuring and organizing a text document, which allows you to code arguments in a standardized way. The core claims and the argument `<Animal suffering>` from above are all formatted in accordance with Argdown conventions.

Argdown-documents can then be read by different programs to automatically generate argument maps or to carry out advanced computations on the argumentative structure.


## Additional Resources

- veggie_deabte.argdown -- The complete reconstruction of the Veggie Debate, as a single Argdown-file.
- http://www.argunet.org -- A blog on argument mapping.
- http://philosophy.hku.hk/think/ -- Free online tutorials and resources on argument analysis.











