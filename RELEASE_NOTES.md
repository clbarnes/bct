<div class="content">

Contents
--------

<div>

-   [Version 2016-16-01: Major update](#1)
-   [Version 2015-25-01: Major update](#2)
-   [Version 2014-04-05: Minor update](#3)

</div>

Version 2016-16-01: Major update[]()
------------------------------------

**New network models**

<div>

-   generative\_model.m: Implements more than 10 generative
    network models.
-   evaluate\_generative\_model.m: Implements and evaluates the accuracy
    of more than 10 generative network models.
-   demo\_generative\_models\_geometric.m and
    demo\_generative\_models\_neighbors.m: Demonstrate the capabilities
    of the new generative model functions.

</div>

**New network measures**

<div>

-   clustering\_coef\_wu\_sign.m: Multiple generalizations of the
    clustering coefficient for networks with positive and
    negative weights.
-   core\_periphery\_dir.m: Optimal core structure and
    core-ness statistic.
-   gateway\_coef\_sign.m: Gateway coefficient (a variant of the
    participation coefficient) for networks with positive and
    negative weights.
-   local\_assortativity\_sign.m: Local (nodal) assortativity for
    networks with positive and negative weights.
-   randmio\_dir\_signed.m: Random directed graph with preserved signed
    in- and out- degree distribution.

</div>

**Removed network measures**

<div>

-   modularity\_louvain\_und\_sign.m, modularity\_finetune\_und\_sign.m:
    This functionality is now provided by community\_louvain.m.
-   modularity\_probtune\_und\_sign.m: Similar functionality is provided
    by consensus\_und.m

</div>

**Bug fixes and/or code improvements and/or documentation improvements**

<div>

-   charpath.m: Changed default behavior, such that infinitely long
    paths (i.e. paths between disconnected nodes) are now included in
    computations by default, but may be excluded manually.
-   community\_louvain.m: Included generalization for negative weights,
    enforced binary network input for Potts-model Hamiltonian,
    streamlined code.
-   eigenvector\_centrality\_und.m: Ensured the use of leading
    eigenvector for computations of eigenvector centrality.
-   modularity\_und.m, modularity\_dir.m: Enforced single node moves
    during fine-tuning step.
-   null\_model\_und\_sign.m and null\_model\_dir\_sign.m: Fixed
    preservation of negative degrees in sparse networks with
    negative weights.
-   randmio\_und\_signed.m: Now allows unbiased exploration of all
    network configurations.
-   transitivity\_bd.m, transitivity\_wu.m, transitivity\_wd.m: removed
    tests for absence of nodewise 3-cycles. Expanded documentation.
-   clustering\_coef\_wu.m, clustering\_coef\_wd.m:
    Expanded documentation.
-   motif3-m and motif4-m functions: Expanded documentation.
-   rich\_club\_wu.m, rich\_club\_wd.m. Expanded documentation.

</div>

**Cosmetic and MATLAB code analyzer (mlint) improvements to many other
functions**

Version 2015-25-01: Major update[]()
------------------------------------

Includes two new community-detection scripts and multiple improvements

<div>

-   New community detection scripts: 1. community\_louvain.m (supersedes
    modularity\_louvain.m and modularity\_finetune.m scripts); 2.
    link\_communities.m.
-   added autofix flag to weight\_conversion.m for fixing common
    weight problems.
-   other function improvements: participation\_coef.m,
    charpath.m, reorder\_mod.m.
-   bug fixes: modularity\_finetune\_und\_sign.m,
    modularity\_probtune\_und\_sign.m, threshold\_proportional.m
-   changed help files: assortativity\_wei.m, distance\_wei.m

</div>

Version 2014-04-05: Minor update[]()
------------------------------------

<div>

-   consensus\_und.m is now a self-contained function
-   headers in charpath.m and in threshold\_proportional.m have been
    corrected

</div>

\
[Published with MATLAB®
R2015b](http://www.mathworks.com/products/matlab/)\

</div>
