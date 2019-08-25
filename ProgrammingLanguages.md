# Programming Languages

  - [x] [Programming Languages - Coursera](https://class.coursera.org/proglang-003)
  - [ ] [Types and Programming Languages - Benjamin C. Pierce](https://www.amazon.com/Types-Programming-Languages-MIT-Press/dp/0262162091)
  - [ ] [Structure and Interpretation of Computer Programs](https://mitpress.mit.edu/sites/default/files/sicp/index.html) or [video series](https://www.youtube.com/watch?v=2Op3QLzMgSY&feature=youtu.be)
  - [ ] [Winter School on Denotational Semantics](https://www.youtube.com/watch?v=EI5i54VrAbc&list=PLvK_yEuhMQ0wxzN_xkkMA4VfFPAjJgnf0)
  - [ ] [Thinking with Types - Type-Level Programming in Haskell](http://thinkingwithtypes.com/)
  - [x] [Inventing Monads - Kabir Shah](https://blog.kabir.sh/posts/inventing-monads.html)
  - [ ] [A reckless introduction to Hindley-Milner type inference
](http://reasonableapproximation.net/2019/05/05/hindley-milner.html)

## [Elm](http://elm-lang.org/)

  - [x] [An Introduction to Elm](https://guide.elm-lang.org/)
  - [x] Build an application
  - [x] [Optimize Elm with Keyed and Lazy](http://elm-lang.org/blog/blazing-fast-html-round-two)
  - [x] [Unit testing](https://github.com/elm-community/elm-test)

## [Haskell](https://www.haskell.org/)

### Haskell - Interested

  - [x] [C9 Lectures: Dr. Erik Meijer - Functional Programming Fundamentals](http://channel9.msdn.com/shows/Going+Deep/Lecture-Series-Erik-Meijer-Functional-Programming-Fundamentals-Chapter-1/)
  - [x] [First 6 chapters of learn you a haskell](http://learnyouahaskell.com/chapters)
  - [x] [99 Problems](http://www.haskell.org/haskellwiki/H-99:_Ninety-Nine_Haskell_Problems) This is great for practicing working with lists and immutability for the first time.
  - [x] [Why Functional Programming Matters](https://www.cs.kent.ac.uk/people/staff/dat/miranda/whyfp90.pdf)

### Haskell - Beginner

  - [x] [DelftX: FP101x Introduction to Functional Programming](https://courses.edx.org/courses/DelftX/FP101x/3T2014/course/) Erik Meijer's course on functional programming.
  - [x] [Programming in Haskell - Graham Hutton](http://www.cs.nott.ac.uk/~pszgmh/pih.html)
      - [x] Monads
  - [x] [Haskell monads and the nest of lies](https://blog.johncs.com/posts/monads-and-how-we-lie.htm) - explains the IO Monad.
  - [x] [Arrays](https://wiki.haskell.org/Modern_array_libraries) and [Vectors](https://wiki.haskell.org/Numeric_Haskell:_A_Vector_Tutorial)
  - [x] Testing
      - [x] [HUnit: Unit testing in haskell](http://hunit.sourceforge.net/)
      - [x] [QuickCheck](http://www.cse.chalmers.se/~rjmh/QuickCheck/): A very cool testing library, based on property based testing. What you do is write a predicate that should always be true `(eg length (reverse list) == length list)`. You then pass the predicate the quickCheck, and it will generate a lot of random values (in this case lists) and test that the predicate is true for all results. [John Hughes - Testing the Hard Stuff and Staying Sane](https://www.youtube.com/watch?v=zi0rHwfiX1Q)
  - [x] Parsing
      - [x] [Parsing stuff in Haskell](https://www.youtube.com/watch?v=r_Enynu_TV0)
      - [x] [Create a parser using Parsec](https://github.com/aslatter/parsec)
  - [x] [Theorems for free!](http://ttic.uchicago.edu/~dreyer/course/papers/wadler.pdf)
  - [x] [Real World Haskell](http://book.realworldhaskell.org/)
      - [x] Monad Transformers
  - [ ] [Continuation passing style](https://en.wikibooks.org/wiki/Haskell/Continuation_passing_style)
  - [ ] [the Continuation monad](http://www.haskellforall.com/2012/12/the-continuation-monad.html)

### Haskell - Moderate

  - [x] Subscribe to [Haskell weekly news](https://haskellweekly.news/)
  - [x] Listen to [The Haskell Cast](https://www.haskellcast.com/)
  - [x] [Do a moderate sized project](https://github.com/katydid/katydid-haskell)
      - [x] Create docs using [haddock](https://www.haskell.org/haddock/)
      - [x] Ask for a community review on [reddit](https://www.reddit.com/r/haskell/comments/78w65f/code_review_request_from_a_noob_haskeller/)
  - [x] [What the heck is Typeable](https://sras.me/haskell/what-the-heck-is-typeable.html)
  - [x] [Fixpoints in Haskell](https://medium.com/@cdsmithus/fixpoints-in-haskell-294096a9fc10)
  - [x] GADTs
  - [x] [Stanford CS240h: Phantoms](http://www.scs.stanford.edu/14sp-cs240h/slides/phantoms.html)
  - [x] [Write foldl using foldr](http://lambda.jstolarek.com/2012/07/expressing-foldl-in-terms-of-foldr/)
  - [ ] Recursion Schemes: catamorphisms, etc.
      - [x] [Understanding F-Algebras](https://bartoszmilewski.com/2013/06/10/understanding-f-algebras/)
      - [x] [An Introduction to Recursion Schemes](http://blog.sumtypeofway.com/an-introduction-to-recursion-schemes/)
      - [x] [Use cata and para for implementing Brzozowski derivatives](https://github.com/awalterschulze/ragax/blob/gh-pages/haskell/deriv/src/FDerive.hs)
      - [ ] [Functional Pearl: Data types a la carte - Wouter Swierstra](http://www.cs.ru.nl/~W.Swierstra/Publications/DataTypesALaCarte.pdf)
  - [x] [Tagless Final Encoding in Haskell](https://jproyo.github.io/posts/2019-03-17-tagless-final-haskell.html)
  - [x] [Inspection Testing](http://hackage.haskell.org/package/inspection-testing)
  - [ ] [Fold and Unfold for Program Semantics - Graham Hutton](http://www.cs.nott.ac.uk/~pszgmh/semantics.pdf)
  - [ ] [A Guide to GHC's Extensions](https://limperg.de/ghc-extensions/)
  - [ ] [Write you a Haskell - Hindley-Milner Inference](http://dev.stephendiehl.com/fun/006_hindley_milner.html)
  - [ ] [Extensible ADT](https://docs.haskus.org/eadt.html)
  - [ ] [data vs codata](https://www.tac-tics.net/blog/data-vs-codata)
  - [ ] [A Tour of Go in Haskell](https://a-tour-of-go-in-haskell.syocy.net/en_US/index.html)
  - [ ] [Linear Haskell: Practical linearity in a higher-order polymorphic language](https://blog.acolyer.org/2018/01/24/linear-haskell-practical-linearity-in-a-higher-order-polymorphic-language/)
  - [ ] Lenses
      - [x] [Haskell Lens - Part 1 - namc.in](https://namc.in/2018-03-26-lenses-part-1)
      - [ ] [Lenses embody Products, Prisms embody Sums](https://blog.jle.im/entry/lenses-products-prisms-sums.html)
  - [ ] Multiparameter type classes/functional dependencie
  - [ ] [Haskell's kind system - a primer](https://diogocastro.com/blog/2018/10/17/haskells-kind-system-a-primer/)
  - [ ] Type families
  - [ ] Existentially quantified types
  - [ ] [Arrows](http://www.haskell.org/arrows/):  Arrows are a way of representing computations that take an input and return an output. A function is the most basic type of arrow, but there are many other types. The library also has many very useful functions for manipulating arrows - they are very useful even if only used with plain old haskell functions.
  - [ ] [Typoclasspedia](https://wiki.haskell.org/Typeclassopedia) Also, there are many concepts (like the Monad concept that you should eventually learn. This will be easier than learning Monads the first time, as your brain will be used to dealing with the level of abstraction involved. A very good overview for learning about these high level concepts and how they fit together is the Typeclassopedia.
  - [ ] [Fast Functional Goats, Lions and Wolves](http://unriskinsight.blogspot.nl/2014/06/fast-functional-goats-lions-and-wolves.html)
  - [ ] [History of Haskell](https://www.microsoft.com/en-us/research/publication/a-history-of-haskell-being-lazy-with-class/?from=http%3A%2F%2Fresearch.microsoft.com%2Fen-us%2Fum%2Fpeople%2Fsimonpj%2Fpapers%2Fhistory-of-haskell%2F)
  - [ ] [What I wish I knew when learning Haskell](http://dev.stephendiehl.com/hask/)

## Conferences

  - [ ] [Lang.NEXT](https://channel9.msdn.com/Events/Lang-NEXT/Lang-NEXT-2014)
  - [x] [International Conference on Functional Programming](https://www.icfpconference.org/)
  - [ ] [StrangeLoop](https://www.thestrangeloop.com/)
  - [ ] [POPL](https://popl18.sigplan.org/)
  
## Scheme
  
  - [x] [The Little Schemer](https://mitpress.mit.edu/books/little-schemer-fourth-edition)
    - Basics of Scheme, Recursion, Higher order functions, Y-combinator and writing an interpreter.
  - [x] [Quote, Unquote - How to Design Programs](https://htdp.org/2018-01-06/Book/i2-3.html)
 
## Erlang

  - [ ] [Learn You Some Erlang for great good](https://learnyousomeerlang.com/)
  
## OCaml

  - [x] [Real World OCaml - Part 1](https://realworldocaml.org/)
    - [ ] Functors
    - [ ] First class Modules
    - [ ] Open recursion
    - [ ] Mixins
  - [ ] [Real World OCaml - Part 2](https://realworldocaml.org/)
  - [ ] [Real World OCaml - Part 3](https://realworldocaml.org/)

## Rust

  - [x] [Programming Rust: Fast, Safe Systems Development](https://www.amazon.co.uk/Programming-Rust-Fast-Systems-Development-ebook/dp/B077NSY211)
  - [ ] [Achieving Warp Speed in Rust](https://gist.github.com/jFransham/369a86eff00e5f280ed25121454acec1)
  
## Lisp

  - [ ] [Lisp in Small Pieces - Book](https://en.m.wikipedia.org/wiki/Lisp_in_Small_Pieces)
  - [ ] [Structure and Interpretation of Computer Programs - Book](https://en.m.wikipedia.org/wiki/Structure_and_Interpretation_of_Computer_Programs)

## Proof Assistants

  - [ ] [Beginner’s Luck: A Language for Property-Based Generators](https://arxiv.org/pdf/1607.05443.pdf)
 
### Pie

  - [x] [The Little Typer](https://mitpress.mit.edu/books/little-typer) and [exercises](https://github.com/awalterschulze/the-little-typer-exercises)

### Coq

  - [ ] [Software Foundations](https://softwarefoundations.cis.upenn.edu/lf-current/toc.html)

### Isabella

  - [ ] [Concrete Semantics](http://www.concrete-semantics.org/)
  
### Agda

  - [ ] [Video Lectures by Conor McBride](https://www.youtube.com/channel/UCWx63QH5IevL6gsP9stpG_w/videos)
  - [ ] [Programming Language Foundations in Agda - Philip Wadler and Wen Kokke](https://plfa.github.io/)
        Starts from the basics and contains a chapter on Bisimulation

### Idris

  - [x] [Idris Tutorial](http://docs.idris-lang.org/en/latest/tutorial/index.html#tutorial-index)

## Logical Programming

  - [ ] [Mercury](https://www.mercurylang.org/)
  - [ ] [TLA+](https://lamport.azurewebsites.net/tla/tla.html)
  - [ ] Prolog

### [miniKanren](http://minikanren.org/)

  - [x] [The Most Beautiful Program Ever Written - William Byrd](https://www.youtube.com/watch?v=OyfBQmvr2Hc)
  - [x] [The Reasoned Schemer](https://mitpress.mit.edu/books/reasoned-schemer)
  - [x] [microKanren: A Minimal Functional Core for Relational Programming](http://webyrd.net/scheme-2013/papers/HemannMuKanren2013.pdf)
  - [x] [Implement it in your favourite programming language](https://github.com/awalterschulze/gominikanren)

## Popular Programming

### Javascript

  - [x] [Douglas Crockford: The JavaScript Programming Language](https://www.youtube.com/watch?v=v2ifWcnQs6M)
  
### Virtual Machines

  - [ ] [One VM to Rule Them All, One VM to Bind Them](https://www.youtube.com/watch?v=FJY96_6Y3a4)
  - [ ] [Graal: How to use the new JVM JIT compiler in real life by Chris Thalinger](https://www.youtube.com/watch?v=_7yIUkP5LiQ&feature=youtu.be)
  - [ ] [Project Sulong: an LLVM bitcode interpreter on the Graal VM with Matthias Grimmer](https://www.youtube.com/watch?v=yyDD_KRdQQU)

### Golang

  - [x] [Effective Go](https://golang.org/doc/effective_go.html)
  - [x] [Go Slices: usage and internals](https://blog.golang.org/go-slices-usage-and-internals)
  - [x] [Profiling Go Programs](https://blog.golang.org/profiling-go-programs)
  - [x] [Functional options for friendly APIs - Dave Cheney](https://dave.cheney.net/2014/10/17/functional-options-for-friendly-apis)
  
### Python

  - [x] [args and kwargs in python explained](https://pythontips.com/2013/08/04/args-and-kwargs-in-python-explained/)
  - [x] [Protocols: Structural subtyping (static duck typing)](https://www.python.org/dev/peps/pep-0544)
