---
author-meta:
- Ryan A. Hagenson
date-meta: '2019-09-16'
keywords:
- biochemistry
- system-f
lang: en-US
title: Biological Calculus
...






<small><em>
This manuscript
([permalink](https://RHagenson.github.io/biological-calculus/v/285ef605ef045dc575ba31cf6df0e334046f36c6/))
was automatically generated
from [RHagenson/biological-calculus@285ef60](https://github.com/RHagenson/biological-calculus/tree/285ef605ef045dc575ba31cf6df0e334046f36c6)
on September 16, 2019.
</em></small>

## Authors



+ **Ryan A. Hagenson**<br>
    ![ORCID icon](images/orcid.svg){.inline_icon}
    [0000-0001-9750-1925](https://orcid.org/0000-0001-9750-1925)
    · ![GitHub icon](images/github.svg){.inline_icon}
    [RHagenson](https://github.com/RHagenson)
    · ![Twitter icon](images/twitter.svg){.inline_icon}
    [RAHagenson](https://twitter.com/RAHagenson)<br>
  <small>
     Department of Conservation Genetics, Omaha's Henry Doorly Zoo and Aquarium
  </small>



## Abstract {.page_break_before}

There must exist a finite set of fundamental operations that define the base of biochemical networks.
The composition of these operations present themselves as the seemingly infinite complexity of biological variety.
If we can determine this finite set of fundamental operations, we might be able to program biochemical networks like we currently program computers.
This paper presents a working theory unifying System F (or _second-order lambda calculus_) with biochemical constraints to build a theoretical framework for defining such a set of finite fundamental operations.


## Introduction

### Biology

Biology is practically the study of exceptions to every rule we write, one need only look to the discovery of extremophiles (citation), the early belief that DNA did not have enough variability to be the code of life (citation), or the multitude of natural examples of the otherwise impossible such as minks' ability to recover from severe skin loss (citation).
With this in mind, let us begin by imagining a perfect species in a perfect world with perfect rules without exceptions -- we can build from there, but trying to build in all (known) exceptions from the start is an impossibility as we have likely not discovered all biological exceptions.
Our perfect species is one that could live immortally within an enclosed system of its own making.
The question then becomes not what our species is, but what it is not.

Things it cannot be:

+ Large bodied: requiring an organ system means failure of any part of the system of specialization results in progression towards mortality
+ Contain memory of function: reliance on a "bank" of functionality in the form of genes cannot be eternally checked for continued validity
+ Permeable: the system must be such that the outside space never perturbs the inside space

### Biochemical Networks

Biochemical networks define a fuzzy boundary such that, within the same space, there exists no barrier for enzymatic access to small molecules -- any enzyme in the same space as a small molecule has some effect on that small molecule and that small molecule has some effect on the enzyme.
This relationship is transitive in that it does not matter if the small molecule is brought to act against the enzyme or the enzyme is brought to act upon the small molecule.
With this fuzziness, a barrier must be enforced where access between the two halves is limited only to those interaction which have some appreciable effect to actualize.

### System F

System F was independently discovered by Jean-Yves Girard @31MrDf8M and John C. Reynolds @CkcfK5kN and is perhaps most notably used by the programming languages Haskell and ML.
As a form of typed lambda calculus, it extends the work of Alfonzo Church @rTK1w3FS, summarized in Table @tbl:lambda-calculus, to allow for parametric polymorphism.
Parametric polymorphism allows for treating similar concrete types generically such that it becomes possible to define operations that work on matches to a unified abstract functional profile (abstract type).

| Syntax  | Name        | Description |
|---------|-------------|-------------|
| $$x$$     | Variable    | A character or string representing a parameter or mathematical/logical value. |
| $$\lambda x.M$$  | Abstraction | Function definition (M is a lambda term). The variable `x` becomes bound in the expression. |
| $$(M N)$$ | Application | Applying a function to an argument. `M` and `N` are lambda terms. |

Table: Alfonzo Church's lambda calculus @UmRc2UHi . {#tbl:lambda-calculus}


## References {.page_break_before}

<!-- Explicitly insert bibliography here -->
<div id="refs"></div>
