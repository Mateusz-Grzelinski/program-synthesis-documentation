Microsoft based research
========================

Web data extraction using hybrid program synthesis
--------------------------------------------------

* Link to paper: `Web data extraction using hybrid program synthesis: a combination of top-down and bottom-up inference <https://www.microsoft.com/en-us/research/publication/web-data-extraction-using-hybrid-program-synthesis-a-combination-of-top-down-and-bottom-up-inference/>`_
* Authors: Mohammad Raza, **Sumit Gulwani**
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
* Authors: Marc Brockschmidt, Miltos Allamanis, Alex Gaunt, **Alex Polozov**
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
* Authors: **Sumit Gulwani**, Prateek Jain
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
* Authors: Mohammad Raza, **Sumit Gulwani**
* Year: 2018
* Discussed problem: improving programming by example (by choosing many top-ranked programs)

* Short description of solution:

    * avoid making a ranking decision at the synthesis stage, instead synthesize a disjunctive program that includes as many possible top-ranked programs as possible alternatives and selects between these different choices upon execution on a new input
    * author gave references to related work about: Ranking based on program structure,Ranking based on additional inputs, Synthesis using richer structures, Conditional Program Synthesis, Neural Program Synthesis, Noise handling

Neural-Guided Deductive Search for Real-Time Program Synthesis from Examples
----------------------------------------------------------------------------

* Link to paper: `Neural-Guided Deductive Search for Real-Time Program Synthesis from Examples <https://www.microsoft.com/en-us/research/publication/neural-guided-deductive-search-real-time-program-synthesis-examples/>`_
* Authors: Ashwin Kalyan, Abhishek Mohta, Alex Polozov, Dhruv Batra, Prateek Jain, **Sumit Gulwani**
* Year: 2018
* Discussed problem: combine symbolic (deductive search) and statistical (machine learning) methods to improve programming by example

* Short description of solution:

    * use machine learning to select grammar rules efficiently
    * propose a program synthesis algorithm that combines key traits of a symbolic and a statistical approach to retain desirable properties like correctness, robust generalization, and real-time performance
    * author gave references to related work about: Neural Program Induction, Neural Program Synthesis, Symbolic Program Synthesis

Learning Natural Programs from a Few Examples in Real-Time
----------------------------------------------------------

* Link to paper: `Learning Natural Programs from a Few Examples in Real-Time <https://www.microsoft.com/en-us/research/publication/learning-natural-programs-from-a-few-examples-in-real-time/>`_
* Authors: Nagarajan Natarajan, Danny Simmons, Naren Datha (narend), Prateek Jain, **Sumit Gulwani**
* Year: 2019
* Discussed problem: programming by example (in  real time, user centric)

    * fact: heuristics in programming by example are often hard to make and not portable

* Short description of solution:

    * author proposes a new technique to embed programs in a vector space making them amenable to ML-formulations
    * author proposes a novel formulation that interleaves program search with ranking, enabling real-time synthesis of accurate user-intended programs

Synthesis and Machine Learning for Heterogeneous Extraction
-----------------------------------------------------------

* Link to paper: `Synthesis and Machine Learning for HeterogeneousExtraction <https://www.microsoft.com/en-us/research/publication/synthesis-and-machine-learning-for-heterogeneous-extraction/>`_
* Authors: Arun Iyer, Manohar Jonnalagedda, Suresh Parthasarathy, Arjun Radhakrishna, **Sriram Rajamani**
* Year: 2019
* Mini glossary: HDEF - Heterogeneous Data Extraction Framework, NoisyDisjSyn - Noisy Disjunctive Program Synthesis
* Discussed problem: combine techniques from the program synthesis and machine learning communities to extract structured information from heterogeneous data (ex. web pages, emails)

* Short description of solution:

    * algorithm:

        1) use machine learning model for initial label extraction (they are noisy)
        2) synthesise program based on labels - it allows for clearing noise
        3) iterate

    * use set of best ranked programs, not only top one
    * author presents algorithm for program synthesis with noisy labels