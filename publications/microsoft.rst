Microsoft based research
========================

Web data extraction using hybrid program synthesis
--------------------------------------------------

* Link to paper: `Web data extraction using hybrid program synthesis: a combination of top-down and bottom-up inference <https://www.microsoft.com/en-us/research/publication/web-data-extraction-using-hybrid-program-synthesis-a-combination-of-top-down-and-bottom-up-inference/>`_
* Authors: Mohammad Raza, Sumit Gulwani
* Year: 2020
* Discussed problem: create program for extracting data (from  web) based on few examples. It can be non formally called automatic web scraping.
* Short description of solution:

    * Combination of top-down and bottom-up synthesis
    * top-down approach provides fast way of satisfying input-output examples given by the user
    * bottom-up approach is unsupervised program synthesis (without user examples) from structure. Systematically enumerating DSL programs and detecting alignment patterns between node selections produced by these programs
    * author proposes way of text-to-node disambiguation for cases where node-based examples cannot be provided

Generative Code Modeling with Graphs
------------------------------------

* Link to paper: `Generative Code Modeling with Graphs <https://www.microsoft.com/en-us/research/publication/generative-code-modeling-with-graphs/>`_
* Authors: Marc Brockschmidt, Miltos Allamanis, Alex Gaunt, Alex Polozov
* Year: 2019
* Discussed problem: studied example is to generate code and fill the hole in program, but paper mentions general concepts:

    * how to represent code as highly structured graph - not only syntax, but also relations are presented ex. last usage of variable
    * generate new, small and expressive code ex. as a hole completion
    * program specification can be provided as input-output examples, natural language, partial program etc.

* Short description of solution:

    * focus on generating graph by extracting code attributes with neural network

Leveraging Grammar and Reinforcement Learning for Neural Program Synthesis
--------------------------------------------------------------------------

* Link to paper: `Leveraging Grammar and Reinforcement Learning for Neural Program Synthesis <https://www.microsoft.com/en-us/research/publication/leveraging-grammar-reinforcement-learning-neural-program-synthesis/>`_
* Authors: Rudy Bunel, Jacob Devlin, Matthew Hausknecht, Rishabh Singh, Pushmeet Kohli
* Year: 2018
* Discussed problem: improvements in existing methods of program synthesis with reinforcement learning:

    * use of syntax checker to guide search
    * problem of program aliasing

* Short description of solution: modifications to objective function, very technical

Programming by Examples: PL meets ML
------------------------------------

* Good article to start - it gives overview what are elements of PBE
* article never explained what is PL in "PL meets ML" :(
* Link to paper: `Programming by Examples: PL meets ML <https://www.microsoft.com/en-us/research/publication/programming-examples-pl-meets-ml/>`_
* Authors: Sumit Gulwani, Prateek Jain
* Year: 2017
* Mini glossary: PBE - programming by example, ML - machine learning, PL - programming language?
* Discussed problem: improve programming by example by pruning search space with machine learning guided heuristics

* Short description of solution:

    * PBE is good for relatively simple well-defined tasks - it produces small, readable code based on few examples
    * ML needs many training data and produces non readable output but handles complex tasks
    * use ML to create ranking function to tell which PBE programs are the most likely

Disjunctive Program Synthesis: A Robust Approach to Programming by Example
--------------------------------------------------------------------------

* Link to paper: `Disjunctive Program Synthesis: A Robust Approach to Programming by Example <https://www.microsoft.com/en-us/research/publication/disjunctive-program-synthesis-a-robust-approach-to-programming-by-example/>`_
* Authors:
* Year:
* Discussed problem:

* Short description of solution:

Neural-Guided Deductive Search for Real-Time Program Synthesis from Examples
----------------------------------------------------------------------------

* Link to paper: `Neural-Guided Deductive Search for Real-Time Program Synthesis from Examples <https://www.microsoft.com/en-us/research/publication/neural-guided-deductive-search-real-time-program-synthesis-examples/>`_
* Authors:
* Year:
* Discussed problem:

* Short description of solution:

Learning Natural Programs from a Few Examples in Real-Time
----------------------------------------------------------

* Link to paper: `Learning Natural Programs from a Few Examples in Real-Time <https://www.microsoft.com/en-us/research/publication/learning-natural-programs-from-a-few-examples-in-real-time/>`_
* Authors:
* Year:
* Discussed problem:

* Short description of solution:

Synthesis and Machine Learning for HeterogeneousExtraction
----------------------------------------------------------

* Link to paper: `Synthesis and Machine Learning for HeterogeneousExtraction <https://www.microsoft.com/en-us/research/publication/synthesis-and-machine-learning-for-heterogeneous-extraction/>`_
* Authors:
* Year:
* Discussed problem:

* Short description of solution:
