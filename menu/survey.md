---
layout: page
title: "Opinion Elicitation"
author: "Sophie v. Schmettow"
---

We define an *opinion* as a *truth-value assignment* to *arguments* featured in a complex debate. Example arguments in case of the Veggie-debate are:

```
1. <Reduce harmful fats>: Animal fats are unhealthy.
   Therefore one should reduce the consumption of 
   animal products as much as possible.
2. <Meat dishes are cultural heritage>:
   Completely abandoning meat and/or animal products
   would put an end to a centuries-old, cultural tra-
   dition – the art of cooking.
3. <Organic only for rich people>: Many people cannot
   afford organic products, especially animal products
   from sustainable agriculture. Organic foods are on-
   ly for rich people.
```

A person can give their opinion by either agreeing to, rejecting or being indifferent towards each of the arguments. For instance, someone could agree to
the first argument, reject the second argument and be indifferent towards the third argument. This opinion can be formalized as a set like this: `{1, !2}`.

A large opinion sample can be gained with the help of an online survey. The survey we constructed from the Veggie-debate can be taken [here](http://i11www.iti.kit.edu/~svschmettow/index.php?lang=en).

In our survey design, we first elicit the participant's core opinion by offering a selection of five options:
* Strictly vegan: You should not eat animal products.
* Strictly vegetarian: You should not eat meat but other animal products are ok.
* Restricted meat consumption: You should restrict meat consumption, e.g. by only buying organic products or by eating meat only occasionally.
* Omnivore: Everybody can eat whatever they like.
* None of the options

On the next page, arguments that are *logically consistent* with the selected option are presented and the participant can indicate for each if (s)he agrees, rejects or is indifferent/has no information about the statement. The last option is the catch-all case where the full set of statements is presented. In case of some of the options, it is possible to give logically inconsistent opinions (for example if a participant agrees that meat consumption should be reduced as much as possible but disagrees that the consumption of animal products should be restriced.) These are not considered on the map. 

## Next Step

After the opinion sample is obtained, an [opinion graph]({{ site.baseurl }}{% link menu/opinion_graph.md %}) is created from it.
