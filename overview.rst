Overview
========
.. _overview:

Entry level, all in one book: `Program Synthesis <https://rishabhmit.bitbucket.io/papers/program_synthesis_now.pdf>`_ by **Sumit Gulwani**, **Oleksandr Polozov**, Rishabh Singh and `follow up blog <https://alexpolozov.com/blog/program-synthesis-2018/>`_

Another github summary `awesome-program-synthesis <https://github.com/praveenkulkarni1996/awesome-program-synthesis>`_

Existing implementations of program synthesis
---------------------------------------------

* `synquid <https://bitbucket.org/nadiapolikarpova/synquid/src/default/src/Synquid/>`_ - haskel, see :ref:`polikarpova_type_guided_synthesis`

    * although synquid is not super complex (~20 files) it is still haskel

* `lambda square <https://github.com/jfeser/L2>`_ (l2) - ocaml - `Synthesizing data structure transformations from input-output examples <https://dl.acm.org/doi/10.1145/2737924.2737977>`_
* `Fiat <http://plv.csail.mit.edu/fiat/>`_ - library for the Coq - `Fiat: Deductive Synthesis of Abstract Data Types in a Proof Assistant <http://adam.chlipala.net/papers/FiatPOPL15/>`_
* `PROSE <https://github.com/microsoft/prose>`_ - C#

    * microsoft baby, production ready framework, of course in C#

* `CEGIS <https://github.com/marcelwa/CEGIS>`_ - c++, see :ref:`counterexample_guided_synthesis`

    * this implementation is one file, super small, uses z3 solver but there is not enough documentation and examples to understand the code...

* Alchemist (code not available?) - `Alchemist: Learning Guarded Affine Functions <https://link.springer.com/chapter/10.1007%2F978-3-319-21690-4_26>`_
* `Sketch <https://people.csail.mit.edu/asolar/>`_ - C++ - `Program Synthesis by Sketching <https://people.csail.mit.edu/asolar/papers/thesis.pdf>`_

    * really nice documentation, custom CEGIS solver (minisat based), custom c based AST, I recommend this project. This is code repair focused solution.

* `SKETCH-N-SKETCH <https://github.com/ravichugh/sketch-n-sketch>`_ - elm - `many papers on official website <https://ravichugh.github.io/sketch-n-sketch/>`_ for example `Sketch-n-Sketch: Output-Directed Programming for SVG <https://arxiv.org/abs/1907.10699>`_
* `STOKE <https://github.com/StanfordPL/stoke>`_ - C++

    * it is well prepared (docs and implementation) code, but the target is super optimization, which can be done by optimizing provided code, or synthesizing new implementation. Not so obvious to use.

* DemoMatch (code not available?) - `DemoMatch: API Discovery from Demonstrations <https://people.csail.mit.edu/asolar/papers/YessenovKS17.pdf>`_
* `PCCoder <https://github.com/amitz25/PCCoder>`_ - python - `Automatic Program Synthesis of Long Programs with a Learned Garbage Collector <https://arxiv.org/abs/1809.04682>`_

    * this is friend of deepcoder, shares DSL. Implementation is surprisingly easy to follow, I recommend this project for starting

* FlashMeta (code not available?) - `FlashMeta:  A  Framework  for  Inductive  Program  Synthesis <https://www.microsoft.com/en-us/research/publication/flashmeta-framework-inductive-program-synthesis/>`_
* `StriSynth <https://github.com/MikaelMayer/StringSolver>`_ - scala - `StriSynth: Synthesis for Live Programming <http://www.cs.yale.edu/homes/piskac/papers/2015GulwaniETALStriSynth.pdf>`_
* `Bayou <https://github.com/capergroup/bayou>`_ - java - `Neural Sketch Learning for Conditional Program Generation <https://arxiv.org/abs/1703.05698>`_
* `Coarse2Fine <https://github.com/donglixp/coarse2fine>`_ - python - `Coarse-to-Fine Decoding for Neural Semantic Parsing <https://www.aclweb.org/anthology/P18-1068/>`_

    * implementation based on `Open-Source Neural Machine Translation Toolkit <https://github.com/OpenNMT/OpenNMT-py>`_, idea based on sketching approach.

* `SemFix <https://github.com/awpandey/SemFix>`_ - C++ - `SemFix: program repair via semantic analysis <https://www.comp.nus.edu.sg/~abhik/pdf/ICSE13-SEMFIX.pdf>`_

    * this is simplistic implementation (5 files), uses z3, minimal documentation

* AutoProf (code not available?) - `<https://excape.cis.upenn.edu/cp_personalized-edu.html#SGS13>`_
* `Rosette <https://github.com/emina/rosette>`_ - `Racket <https://racket-lang.org/>`_ (general purpose language oriented programming language) - solver-aided programming language that extends with language constructs for program synthesis, verification
* `strans <https://github.com/Inventitech/strans>`_ - small shell utility for string manipulation using prose SDK
* `AI-Programmer <https://github.com/primaryobjects/AI-Programmer>`_ - c# - experiment with using artificial intelligence and genetic algorithms to automatically generate programs
* `suggest.el <https://github.com/Wilfred/suggest.el>`_ - emacs lisp - discover elisp functions based on examples
* `Cozy <https://github.com/CozySynthesizer/cozy>`_ - python - synthesize data structure implementations from simple high-level specifications
* `Metagol <https://github.com/metagol/metagol>`_ - prolog - inductive logic programming (ILP) system based on meta-interpretive learning
* `NEAR Program Synthesis <https://github.com/nearai/program_synthesis>`_ - python, jupyter notebook - set of models, tools, and datasets for program synthesis tasks
* `Neural Symbolic Machines (NSM) <https://github.com/crazydonkey200/neural-symbolic-machines>`_ - python, jypyter notebook - framework to integrate neural networks and symbolic representations using reinforcement learninframework to integrate neural networks and symbolic representations using reinforcement learningg

Programs from sygus:

* `CVC4 <https://cvc4.github.io>`_ - c++ - `CVC4SY: Smart and Fast Term Enumeration for Syntax-Guided Synthesis <http://homepage.divms.uiowa.edu/~hbarbosa/papers/cvc4sygus.pdf>`_. `CVC4 wiki <https://github.com/CVC4/CVC4/wiki>`_ has some valuable links
* `DeepCoder <https://github.com/dkamm/deepcoder>`_ - python -  `DeepCoder: Learning to Write Programs <https://www.microsoft.com/en-us/research/publication/deepcoder-learning-write-programs/>`_
* `DryadSynth <https://github.rcac.purdue.edu/cap/DryadSynth>`_ - java - `DRYADSYNTH: A Concolic SyGuS Solver <https://engineering.purdue.edu/~xqiu/DryadSynth.pdf>`_
* `LoopInvGen  <https://github.com/SaswatPadhi/LoopInvGen>`_ - omcaml - `LoopInvGen: A Loop Invariant Generator based on Precondition Inference <https://arxiv.org/abs/1707.02029>`_
* EUSolver (code not available?) - `Scaling Enumerative Program Synthesis via Divide and Conquer <https://www.cis.upenn.edu/~alur/Tacas17.pdf>`_
* ICE-DT (code not available?) - `ICE: A robust framework for learning invariants <https://link.springer.com/chapter/10.1007/978-3-319-08867-9_5>`_
* OASIS (code not available?) - `OASIS: ILP-Guided Synthesis of Loop Invariants <https://arxiv.org/abs/1911.11728>`_
* `Euphony <https://github.com/wslee/euphony>`_ - python

Other projects, not directly connected to program synthesis:

* `Code2Vec <https://github.com/tech-srl/code2vec>`_ or newer `Code2Seq <https://github.com/tech-srl/code2seq>`_ and newest `AnyCodeGen <https://anycodegen.org/>`_

    * this code comes from same authors, it is ok but it is slow to work with. Each of projects touches a bit different field of use of code in ML. They use tensorflow 1 (although you can find 2 port). They provide pretrained models, so plug and play solution is not that bad, but it is still cumbersome, as this is not meant to be library. Documentation is ok. Training your own model is a pain because you need to preprocess your language (python, java, ...) into universal AST (AST itself is not super well documented), it is slow as hell.

Authors worth looking into
--------------------------

* `Sriram Rajamani <https://www.microsoft.com/en-us/research/people/sriram/>`_ - **Advanced course on program synthesis by among others Sriram Rajamani:** `<https://www.csa.iisc.ac.in/~deepakd/psml-2020/>`_
* `Alex Polozov <https://alexpolozov.com/>`_

Other articles
==============

* https://blog.sigplan.org/2019/08/22/from-programs-to-deep-models-part-1/
* https://blog.sigplan.org/2020/02/12/from-programs-to-deep-models-part-2/
* https://blog.sigplan.org/2020/05/11/from-programs-to-deep-models-part-3-code-completion/
