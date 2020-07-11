Code repair
===========

The biggest challenge in code repair is code representation. It is similar to natural language processing as it has sequence-to-sequence character


Code2vec & Code2Seq & AnyCodeGen
--------------------------------

* This is incremental work from same authors, featured at conferences
* Problem: learn code distribution (for various uses in machine learning)
* Authors: Uri Alon, Shaked Brody, Omer Levy and Eran Yahav
* Link to demos (with link to papers and code): https://code2vec.org, https://code2seq.org, https://anycodegen.org/

    * the code is good quality, but is really hard do work with. There is a lot of preprocessing, and tensorflow code is level-expert

* Short description of solution:

    * code2vec: Learning Distributed Representations of Code:

        * represent a code snippet as a single fixed-length code vector. This vector can be used for predictions in ML
        * to achieve this code is first decomposed to a collection of paths in its abstract syntax tree
        * network learns the atomic representation of each path while simultaneously learning how to aggregate a set of them

    * code2seq: generating sequences from structured representation of code:

        * generate natural language sequences from source code snippets
        * represents a code snippet as the set of paths
        * use LSTM so learn code distribution

    * AnyCodeGen - SLM: Structural Language Models of Code

        * any-code completion
        * demo completes code :)

