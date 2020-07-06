Code repair
===========

The biggest challenge in code repair is code representation. It is similar to natural language processing as it has sequence-to-sequence character

* nice blog posts:

    * https://blog.sigplan.org/2019/08/22/from-programs-to-deep-models-part-1/
    * https://blog.sigplan.org/2020/02/12/from-programs-to-deep-models-part-2/
    * https://blog.sigplan.org/2020/05/11/from-programs-to-deep-models-part-3-code-completion/

Code2vec & Code2Seq & AnyCodeGen
--------------------------------

* This is incremental work from same authors, featured at conferences
* Problem: learn code distribution (for use in machine learning)
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
