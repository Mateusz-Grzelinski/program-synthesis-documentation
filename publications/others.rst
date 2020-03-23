Other researchers
=================

Program Synthesis by Type-Guided Abstraction Refinement
-------------------------------------------------------

* continuation of `Resource-Guided Program Synthesis <https://cseweb.ucsd.edu/~npolikarpova/publications/pldi19.pdf>`_ `<ReSyn demo <http://comcom.csail.mit.edu/comcom/#ReSyn>`_
* Authors: `Nadia Polikarpova <https://cseweb.ucsd.edu/~npolikarpova/>`_, Ivan KurajArmando, Solar-Lezama
* Year: 2020
* Link to paper: `Program Synthesis from Polymorphic Refinement Types <https://cseweb.ucsd.edu/~npolikarpova/publications/pldi16.pdf>`_
* Discussed problem: program synthesis (with recursive functions) by specification. Output program is guaranteed to be correct.
* Short description of solution:

    * use haskel like syntax to define program constrains (reduce search space), instead of logical formal language
    * use of refinement types to decrease search space: :code:`{x:Int | 0 < x}` - :code:`x` is always less than 0. Type defined with predicate  is called Logically Qualified Data Types - `Liquid Types <http://goto.ucsd.edu/~rjhala/liquid/liquid_types.pdf>`_

* their solver is called Synquid - "SYNthesis with liQUIDtypes" (`Synquid demo <http://comcom.csail.mit.edu/comcom/#Synquid>`_)

Interactive Program Synthesis
-----------------------------

* Link to paper `Interactive Program Synthesis <https://arxiv.org/abs/1703.03539>`_
* Authors:
* Year:
* Discussed problem:

* Short description of solution:
