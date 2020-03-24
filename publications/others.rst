Other researchers
=================

.. _polikarpova_type_guided_synthesis:

Program Synthesis by Type-Guided Abstraction Refinement
-------------------------------------------------------

* Indirect continuation of `Resource-Guided Program Synthesis <https://cseweb.ucsd.edu/~npolikarpova/publications/pldi19.pdf>`_ `<ReSyn demo <http://comcom.csail.mit.edu/comcom/#ReSyn>`_ (same author)
* Authors: `Nadia Polikarpova <https://cseweb.ucsd.edu/~npolikarpova/>`_, Ivan KurajArmando, Solar-Lezama
* Year: 2020
* Link to paper: `Program Synthesis from Polymorphic Refinement Types <https://cseweb.ucsd.edu/~npolikarpova/publications/pldi16.pdf>`_
* Discussed problem: program synthesis (with recursive functions) by formal specification
* Short description of solution:

    * use haskel like syntax to define program constrains (reduce search space), instead of logical formal language
    * use of refinement types to decrease search space: :code:`{x:Int | 0 < x}` - :code:`x` is always less than 0. Type defined with predicate  is called Logically Qualified Data Types - `Liquid Types <http://goto.ucsd.edu/~rjhala/liquid/liquid_types.pdf>`_

* their solver is called Synquid - "SYNthesis with liQUIDtypes" (`Synquid demo <http://comcom.csail.mit.edu/comcom/#Synquid>`_)

.. _counterexample_guided_synthesis:

Counterexample Guided Inductive Synthesis Modulo Theorie
--------------------------------------------------------

* Link to paper `Counterexample Guided Inductive Synthesis Modulo Theorie <http://www.kroening.com/papers/cav2018-synthesis.pdf>`_
* Autors:  Alessandro Abate, Cristina David, Pascal Kesseli, Daniel Kroening, Elizabeth Polgreen
* Year: 2018
* Discussed problem: programming by formal specification

    * improve speed with approach called CEGIS - CounterExample Guided Inductive Synthesis
    * generation of programs that require non-trivial constants

* Short description of solution:

Syntax-Guided Synthesis
-----------------------

* Good overview of approaches (no ML based approaches included)
* Link to paper: `Syntax-Guided Synthesis <https://www.cis.upenn.edu/~fisman/documents/SyGuS_JournalVersion.pdf>`_
* `Syntax Guided synthesis competition SyGus <https://sygus.org/>`_  competition formal definition [#]_
* Authors: Rajeev Alur, Rastislav Bodik, Eric Dallal, Dana Fisman,Pranav Garg, Garvit Juniwal, Hadas Kress-Gazit, P. Madhusudan, Milo M. K. Martin, Mukund Raghothaman, Shamwaditya Saha, Sanjit A. Seshia, Rishabh Singh, Armando Solar-Lezama, Emina Torlak and Abhishek Udupa
* Year: 2013
* Discussed problem: program synthesis in syntax guided approach. Review of existing solutions
* Short description of solution:

.. [#] side note: similar idea is `The Reactive Synthesis Competition <http://www.syntcomp.org/>`_

Proving Unrealizability for Syntax-Guided Synthesis
---------------------------------------------------

* Featured at CAV (Computer-Aided Verification conference) 2019
* Link to paper: `Proving Unrealizability for Syntax-Guided Synthesis <https://link.springer.com/chapter/10.1007/978-3-030-25540-4_18>`_
* Authors: Qinheping Hu, Jason Breck, John Cyphert, Loris D’Antoni and Thomas Reps1
* Year: 2019
* Discussed problem:
* Short description of solution:

Overfitting in Synthesis: Theory and Practice
---------------------------------------------

* Featured at CAV 2019
* Link to paper `Overfitting in Synthesis: Theory and Practice <https://link.springer.com/chapter/10.1007%2F978-3-030-25540-4_17>`_
* Authors: Saswat PadhiEmail, Todd Millstein, Aditya Nori, Rahul Sharma

Efficient Synthesis with Probabilistic Constraints
--------------------------------------------------

* Featured at CAV 2019
* Link to paper: `Efficient Synthesis with Probabilistic Constraints <https://link.springer.com/chapter/10.1007%2F978-3-030-25540-4_15>`_
* Year: 2019
* Authors: Samuel Drews, Aws Albarghouthi, Loris D’Antoni
* Discussed problem: program synthesis, when constrains are given by probability
