* Text _and_ Loop Text
  - Loop Text is Text with an index. The GC can know enough to collect the parts of a string that aren't pointed to
  - Loop Text is really (Int, Text) so:
    loopify :: Text -> Loop Text
    loopify t = (0,t) 

    deloop :: Loop Text -> Text
    deloop (0, t) = t
    deloop (n, t) = drop n t

* Local Data types

* System D-like notion of dependent types

* Qualified do

* Constrained Monads as default

* Indexed Monads provided as 'batteries included', but not part of the prelude.

* IO has notion of lifetimes (FFI with Rust)

* Generic programming powerful enough to define Show

* Syntax:
  - Trailing Commas (generalized?):
  - function : Type
  - string literals have different begin and end symbols
  - String interpolation

* Modules are Haskell-like but with renaming
