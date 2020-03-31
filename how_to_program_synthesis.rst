How to program synthesis
========================

There are 3 components in program synthesis:

1) Domain specific language - DSL
2) Specification of expected output, for example:

    * formal logic specification,
    * by input-output example - PBE - programming by example,
    * by providing code snippet

3) Solver (search method)

Applications
------------

* data wrangling, for example:

    * automatic web scraping
    * extracting data from logs, json, xml
    * transformations, for example:

        * transforming date, string, number formats
        * transforming tables

* graphics

    * automating copy paste tasks
    * combining direct manipulation of graphical elements and constraint system

* code repair

    * automatic homework checking

* code suggestions

    * automatic discovery of API
    * next generation code suggestions

* superoptimization
* concurrent programming

General principles
------------------

* enumerative

    * top-down
    * bottom-up
    * Bidirectional - combine 2 above
    * Offline Exhaustive Enumeration and Composition - pregenerate all possible programs up to some point.

* sketching - mimic real life approach to programming: first create sketch (partial high level solution) and then implement
* syntax-guided synthesis - use syntax to prune search space
* type-guided synthesis - use type information to prune search space
* DSL - choose wisely based on expressivity, choice of operators, naturalness, efficiency

Optimizations:

* Markov Chain Monte CarloMCMC techniques in program synthesis employ a variation of genetic programming, where Metropolis-Hastings algorithm is used to explore a search space of possible programs. In MCMC sampling, we aim to draw programs from the space with prob-ability proportional to their cost
* Version Space Algebra - VSA - offer a succinct representation of the program space that is amenable to structure-based ranking
* Machine Learning - ML - various uses, from end-to-end synthesis to choosing best step based on learned model
* Metasketch - metasketch is a generalization of a sketch. Instead of a single partial program, it gives an ordered family of such partial programs, along with a cost function and a gradient

