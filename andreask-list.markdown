* Local Data types

* Local instances (?) (explicit dictionary passing?)

* Haskell-like types system (GADTs)

* Unlifted data types should be 'closer to first class' than in Haskell
  - The user should have control of whether something is lazy or not.
    e.g. "for this function, the body can assume that arguments are strict"

* Opt-in 'liftedness polymorphism'

* Strings should be behind some abstraction.

* Believe that Backpack goes in the right direction.
  - User should be able to instantiate an API at a specified type.

* More ways to get guarantees from the compiler
  - write function once and have it be a compiler error if it fails to specialize.

* Fields of ADTs should be strict by default. Opt-in for laziness.

* Standard code formatter (rustfmt)

* Compiler should be designed with Language-server use-cases

* known-to-be-compile-time expressions.
