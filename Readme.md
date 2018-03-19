A list of videos, playlists, blog posts, papers, books, etc that I have learned from and still intend to learn from.

# Programming Languages

## Parsing and Automata

  - [x] [Tree Automata and Tree Grammars - Joost Engelfriet](https://arxiv.org/pdf/1510.02036.pdf)
  - [x] [Learn You a gocc for Great Good - Marius Ackerman](https://raw.githubusercontent.com/goccmack/gocc/master/doc/gocc_user_guide.pdf)
  - [x] [Parsing Expression Grammars: A Recognition-Based Syntactic Foundation](http://bford.info/pub/lang/peg.pdf)
  - [x] [Combinator Parsers A Short Tutorial](http://www.cs.uu.nl/research/techreps/repo/CS-2008/2008-044.pdf)
  - [x] [Lecture 6: Alternating Automata](http://www.cmi.ac.in/~kumar/words/lecture06.pdf)
  - [x] [Regular-expression derivatives reexamined](https://people.mpi-sws.org/~turon/re-deriv.pdf)
  - [x] [Parsing with Derivatives - a functional pearl - Matthew Might, David Darais and Daniel Spiewak](https://s3.amazonaws.com/academia.edu.documents/30626123/might2011derivatives.pdf?AWSAccessKeyId=AKIAIWOWYYGZ2Y53UL3A&Expires=1518892310&Signature=h%2BGIOGvJDelNj2jLucDwIHGO7kc%3D&response-content-disposition=inline%3B%20filename%3DParsing_with_derivatives_a_functional_pe.pdf)
  - [x] [Visibly Pushdown Languages - Rajeev Alur and P Madhusudan](https://repository.upenn.edu/cgi/viewcontent.cgi?article=1174&context=cis_papers)
  - [x] [High-Performance Complex Event Processing over XML Streams - Barzan Mozafari, Kai Zeng, Carlo Zaniolo](http://web.cs.ucla.edu/~zaniolo/papers/p253-mozafari.pdf)
  - [x] [Visibly Pushdown Automata for Streaming XML - Varij Kumar, P Madhusdan, Mahesh Viswanathan](http://www.ra.ethz.ch/cdstore/www2007/www2007.org/papers/paper788.pdf)
  - [x] [Regular Expression Sub-Matching using Partial Derivatives - Martin Sulzmann and Kenny Zhuo Ming Lu](https://5b6c6881-a-62cb3a1a-s-sites.googlegroups.com/site/luzhuomi/file/ppdp39-sulzmann.pdf?attachauth=ANoY7crz7zlgeFVqKfz21xs3J43HwF_-sNbCMgfXTF_n3NGvtRj9c38uRQfo-0djC_uj60Hwfg0UCE21pwBzsG0Tp6g5PG1_Bbc0Pua71Gw9_rDuGmxecsdMhf9QgdCh6KsqVLFmBr2PyasKYi29DzgyCBRzJiIEjeNKMNHlHlDrodJ80qwFUrh46HVlQn8IJOorscdZn9J6rgi0uoX6UQmqfzBltBSOOjCi0sVx8_s8NPrrtEpbq3o%3D&attredirects=0)
  - [x] [Correct and Efficient POSIX Submatch Extraction with Regular Expression Derivatives - Martin Sulzmann and Kenny Zhuo Ming Lu](http://www.home.hs-karlsruhe.de/~suma0002/publications/posix-derivatives.pdf)
  - [x] [Taxonomy of XML Schema Languages Using Formal Language Theory - Makoto Murata](https://www.tjhsst.edu/~rlatimer/acm/InternetTechnology/XMLFormalLanguagep660-murataTOITNov05.pdf)
  - [x] [Foundations of XML Processing: The Tree Automata Approach - Haruo Hosoya](http://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.138.6773&rep=rep1&type=pdf)
  - [ ] [Restricting Grammars with Tree Automata - Michael D. Adams and Matthew Might](http://delivery.acm.org/10.1145/3140000/3133906/oopsla17-oopsla234.pdf?ip=62.195.23.191&id=3133906&acc=OA&key=4D4702B0C3E38B35%2E4D4702B0C3E38B35%2EFF4855CDBAECEBC5%2EC1E31BC46E58D5B8&__acm__=1518888271_476e608b6be1213e8e1bfb39669d33c5)
  - [ ] [Verified Decision Procedures for MSO on Words Based on Derivatives of Regular Expressions](https://www21.in.tum.de/~traytel/papers/icfp13-mso/index.html)

## [Elm](http://elm-lang.org/)

  - [x] [An Introduction to Elm](https://guide.elm-lang.org/)
  - [x] Build an application
  - [x] [Optimize Elm with Keyed and Lazy](http://elm-lang.org/blog/blazing-fast-html-round-two)
  - [ ] [Debug](http://debug.elm-lang.org/)
  - [ ] [Time Traveling made easy](http://elm-lang.org/blog/time-travel-made-easy)
  - [x] [Unit testing](https://github.com/elm-community/elm-test)

## [Haskell](https://www.haskell.org/)

### Haskell - Beginner

  - [x] [Programming in Haskell - Graham Hutton](http://www.cs.nott.ac.uk/~pszgmh/pih.html)
  - [x] ~~[C9 Lectures: Dr. Erik Meijer - Functional Programming Fundamentals](http://channel9.msdn.com/shows/Going+Deep/Lecture-Series-Erik-Meijer-Functional-Programming-Fundamentals-Chapter-1/)~~
  - [x] ~~[First 6 chapters of learn you a haskell](http://learnyouahaskell.com/chapters)~~
  - [x] [DelftX: FP101x Introduction to Functional Programming](https://courses.edx.org/courses/DelftX/FP101x/3T2014/course/) Erik Meijer's course on functional programming.
  - [x] [99 Problems](http://www.haskell.org/haskellwiki/H-99:_Ninety-Nine_Haskell_Problems) This is great for practicing working with lists and immutability for the first time.
  - [x] [Why Functional Programming Matters](https://www.cs.kent.ac.uk/people/staff/dat/miranda/whyfp90.pdf)
  - [x] [HUnit: Unit testing in haskell](http://hunit.sourceforge.net/)
  - [x] [QuickCheck](http://www.cse.chalmers.se/~rjmh/QuickCheck/): A very cool testing library, based on property based testing. What you do is write a predicate that should always be true `(eg length (reverse list) == length list)`. You then pass the predicate the quickCheck, and it will generate a lot of random values (in this case lists) and test that the predicate is true for all results. [John Hughes - Testing the Hard Stuff and Staying Sane](https://www.youtube.com/watch?v=zi0rHwfiX1Q)
  - [x] [Parsing stuff in Haskell](https://www.youtube.com/watch?v=r_Enynu_TV0)
  - [x] [Create a parser using Parsec](https://github.com/aslatter/parsec)
  - [x] [Theorems for free!](http://ttic.uchicago.edu/~dreyer/course/papers/wadler.pdf)
  - [x] ~~[Real World Haskell](http://book.realworldhaskell.org/)~~
  - [ ] [Continuation passing style](https://en.wikibooks.org/wiki/Haskell/Continuation_passing_style)
  - [ ] [the Continuation monad](http://www.haskellforall.com/2012/12/the-continuation-monad.html)

### Haskell - Moderate

  - [x] [Do a moderate sized project](https://github.com/katydid/katydid-haskell)
  - [x] Create docs using [haddock](https://www.haskell.org/haddock/)
  - [x] Ask for a community review on [reddit](https://www.reddit.com/r/haskell/comments/78w65f/code_review_request_from_a_noob_haskeller/)
  - [ ] [An Introduction to Recursion Schemes](http://blog.sumtypeofway.com/an-introduction-to-recursion-schemes/)
  - [ ] [Fold and Unfold for Program Semantics - Graham Hutton](http://www.cs.nott.ac.uk/~pszgmh/semantics.pdf)
  - [ ] [data vs codata](https://www.tac-tics.net/blog/data-vs-codata)
  - [ ] [A Tour of Go in Haskell](https://a-tour-of-go-in-haskell.syocy.net/en_US/index.html)
  - [ ] [Linear Haskell: Practical linearity in a higher-order polymorphic language](https://blog.acolyer.org/2018/01/24/linear-haskell-practical-linearity-in-a-higher-order-polymorphic-language/)
  - [x] Subscribe to [Haskell weekly news](https://haskellweekly.news/)
  - [ ] Multiparameter type classes/functional dependencie
  - [ ] Type families
  - [ ] Existentially quantified types
  - [ ] Phantom types
  - [x] GADTs
  - [ ] [Arrays](https://wiki.haskell.org/Modern_array_libraries): the various mutable/immutable arrays
  - [ ] [Arrows](http://www.haskell.org/arrows/):  Arrows are a way of representing computations that take an input and return an output. A function is the most basic type of arrow, but there are many other types. The library also has many very useful functions for manipulating arrows - they are very useful even if only used with plain old haskell functions.
  - [ ] [Typoclasspedia](https://wiki.haskell.org/Typeclassopedia) Also, there are many concepts (like the Monad concept that you should eventually learn. This will be easier than learning Monads the first time, as your brain will be used to dealing with the level of abstraction involved. A very good overview for learning about these high level concepts and how they fit together is the Typeclassopedia.
  - [ ] Do Haskell Web development
  - [ ] [Popular Haskell Libraries](https://haskell.zeef.com/konstantin.skipor)
  - [ ] [Fast Functional Goats, Lions and Wolves](http://unriskinsight.blogspot.nl/2014/06/fast-functional-goats-lions-and-wolves.html)
  - [ ] [History of Haskell](https://www.microsoft.com/en-us/research/publication/a-history-of-haskell-being-lazy-with-class/?from=http%3A%2F%2Fresearch.microsoft.com%2Fen-us%2Fum%2Fpeople%2Fsimonpj%2Fpapers%2Fhistory-of-haskell%2F)
  - [ ] [What I wish I knew when learning Haskell](http://dev.stephendiehl.com/hask/)
  - [ ] [Functional Programming with Bananas, Lenses, Envelopes and Barbed Wire](https://maartenfokkinga.github.io/utwente/mmf91m.pdf)

## Maths

  - [ ] [3Blue1Brown - Neat proofs/perspectives](https://www.youtube.com/playlist?list=PLZHQObOWTQDPSKntUcMArGheySM4gL7wS)
  - [ ] [euclideanspace - Maths - Abstract Algebra and Discrete Mathematics](http://euclideanspace.com/maths/discrete/index.htm)

### Discrete Maths

  - [x] [Discrete Mathematics for Computer Science: Logic](http://people.cs.pitt.edu/~milos/courses/cs441/lectures/Class1.pdf)
  - [x] [Discrete Mathematics for Computer Science: Propositional logic](http://people.cs.pitt.edu/~milos/courses/cs441/lectures/Class2.pdf)
  - [ ] [Discrete Mathematics for Computer Science: Predicate logic](http://people.cs.pitt.edu/~milos/courses/cs441/lectures/Class3.pdf)
  - [ ] [Discrete Mathematics for Computer Science: Class4](http://people.cs.pitt.edu/~milos/courses/cs441/lectures/Class4.pdf)
  - [ ] [Discrete Mathematics for Computer Science: Class5](http://people.cs.pitt.edu/~milos/courses/cs441/lectures/Class5.pdf)
  - [ ] [Discrete Mathematics for Computer Science: Class6](http://people.cs.pitt.edu/~milos/courses/cs441/lectures/Class6.pdf)
  - [ ] [Discrete Mathematics for Computer Science: Class7](http://people.cs.pitt.edu/~milos/courses/cs441/lectures/Class7.pdf)
  - [ ] [Discrete Mathematics for Computer Science: Class8](http://people.cs.pitt.edu/~milos/courses/cs441/lectures/Class8.pdf)
  - [ ] [Discrete Mathematics for Computer Science: Class9](http://people.cs.pitt.edu/~milos/courses/cs441/lectures/Class9.pdf)
  - [ ] [Discrete Mathematics for Computer Science: Class10](http://people.cs.pitt.edu/~milos/courses/cs441/lectures/Class10.pdf)
  - [ ] [Discrete Mathematics for Computer Science: Class11](http://people.cs.pitt.edu/~milos/courses/cs441/lectures/Class11.pdf)
  - [ ] [Discrete Mathematics for Computer Science: Class12](http://people.cs.pitt.edu/~milos/courses/cs441/lectures/Class12.pdf)
  - [ ] [Discrete Mathematics for Computer Science: Class13](http://people.cs.pitt.edu/~milos/courses/cs441/lectures/Class13.pdf)
  - [ ] [Discrete Mathematics for Computer Science: Class14](http://people.cs.pitt.edu/~milos/courses/cs441/lectures/Class14.pdf)
  - [ ] [Discrete Mathematics for Computer Science: Class15](http://people.cs.pitt.edu/~milos/courses/cs441/lectures/Class15.pdf)
  - [ ] [Discrete Mathematics for Computer Science: Class16](http://people.cs.pitt.edu/~milos/courses/cs441/lectures/Class16.pdf)
  - [ ] [Discrete Mathematics for Computer Science: Class17](http://people.cs.pitt.edu/~milos/courses/cs441/lectures/Class17.pdf)
  - [ ] [Discrete Mathematics for Computer Science: Class18](http://people.cs.pitt.edu/~milos/courses/cs441/lectures/Class18.pdf)
  - [ ] [Discrete Mathematics for Computer Science: Class19](http://people.cs.pitt.edu/~milos/courses/cs441/lectures/Class19.pdf)
  - [ ] [Discrete Mathematics for Computer Science: Class20](http://people.cs.pitt.edu/~milos/courses/cs441/lectures/Class20.pdf)
  - [ ] [Discrete Mathematics for Computer Science: Class21](http://people.cs.pitt.edu/~milos/courses/cs441/lectures/Class21.pdf)
  - [ ] [Discrete Mathematics for Computer Science: Class22](http://people.cs.pitt.edu/~milos/courses/cs441/lectures/Class22.pdf)
  - [ ] [Discrete Mathematics for Computer Science: Class23](http://people.cs.pitt.edu/~milos/courses/cs441/lectures/Class23.pdf)
  - [ ] [Discrete Mathematics for Computer Science: Class24](http://people.cs.pitt.edu/~milos/courses/cs441/lectures/Class24.pdf)
  - [ ] [Discrete Mathematics for Computer Science: Class25](http://people.cs.pitt.edu/~milos/courses/cs441/lectures/Class25.pdf)
  - [ ] [Discrete Mathematics for Computer Science: Class26](http://people.cs.pitt.edu/~milos/courses/cs441/lectures/Class26.pdf)

### Abstract Algebra

  - [x] [Abstract Algebra on Socratica](https://www.youtube.com/playlist?list=PLi01XoE8jYoi3SgnnGorR_XOW3IcK-TP6)

### Category Theory

  - [x] [Category Theory for Programmers 1](https://www.youtube.com/playlist?list=PLbgaMIhjbmEnaH_LTkxLI7FMa2HsnawM_)
  - [ ] [Category Theory for Programmers blog](https://bartoszmilewski.com/2014/10/28/category-theory-for-programmers-the-preface/) - [My Answers to Challenges](https://github.com/awalterschulze/category-theory-for-programmers-challenges)
  - [ ] [Category Theory for Programmers 2](https://www.youtube.com/playlist?list=PLbgaMIhjbmElia1eCEZNvsVscFef9m0dm)

### Coalgebra

  - [x] [Automata and Coinduction (an exercise in coalgebra) - J.J.M.M Rutten](https://fldit-www.cs.uni-dortmund.de/~peter/Rutten/AutomataCoind.pdf)
  - [x] [A Tutorial on Coalgebras and Coinduction](https://pdfs.semanticscholar.org/40bb/e9978e2c4080740f55634ac58033bfb37d36.pdf)
  - [ ] [Kleene Coalgebra: an overview - Alexandra Silva, Marcello Bonsangue and Jan Rutten](https://homepages.cwi.nl/~janr/papers/files-of-papers/2011-nvti.pdf)
  - [ ] [Fundamental Study: Universal Coalgebra: A theory of systems](http://www.sciencedirect.com/science/article/pii/S0304397500000566)
  - [ ] [The basics of coinduction - Jan Stolarek](http://lambda.jstolarek.com/2015/03/the-basics-of-coinduction/)
  
### Logic

  - [ ] [Monadic Second Order Logic](https://cs.stackexchange.com/questions/82994/monadic-second-order-logic-for-dummies)

### Homotopy Type Theory

  - [ ] [Homotopy Type Theory](http://%0Ahttp://www.cs.cmu.edu/~rwh/courses/hott/)

## Conferences

  - [ ] [Lang.NEXT](https://channel9.msdn.com/Events/Lang-NEXT/Lang-NEXT-2014)
  - [x] [International Conference on Functional Programming](https://www.icfpconference.org/)
  - [ ] [StrangeLoop](https://www.thestrangeloop.com/)
  - [ ] [POPL](https://popl18.sigplan.org/)

## Courses

  - [x] [Programming Languages](https://class.coursera.org/proglang-003)
  - [ ] [Intro to Theoretical Computer Science](https://www.udacity.com/course/intro-to-theoretical-computer-science--cs313)

## Rust

  - [ ] [Achieving Warp Speed in Rust](https://gist.github.com/jFransham/369a86eff00e5f280ed25121454acec1)

## Curated Lists

  - [ ] [Awesome Compilers](https://github.com/aalhour/awesome-compilers)

## Types

  - [ ] [Type Theory Foundations](https://www.youtube.com/playlist?list=PLGCr8P_YncjXRzdGq2SjKv5F2J8HUFeqN)
  - [ ] [Types and Programming Languages](https://www.cis.upenn.edu/~bcpierce/tapl/)
  - [ ] [Practical Foundations for Programming Languages](https://www.cs.cmu.edu/~rwh/pfpl/2nded.pdf)
  - [ ] [Oleg Kiselyov's site](http://okmij.org/ftp/)
  - [ ] [Adventures with Types](https://www.youtube.com/watch?v=6COvD8oynmI)
  - [ ] [SQL in the type system where it belongs](http://ren.zone/articles/opaleye-sot)
  - [ ] [Structural type system](https://en.wikipedia.org/wiki/Structural_type_system)

## Proof Assistants

 - [ ] [Beginner’s Luck: A Language for Property-Based Generators](https://arxiv.org/pdf/1607.05443.pdf)

### Coq

  - [ ] [Software Foundations](https://softwarefoundations.cis.upenn.edu/lf-current/toc.html)

### Isabella

  - [ ] [Concrete Semantics](http://www.concrete-semantics.org/)

### Idris

  - [x] [Idris Tutorial](http://docs.idris-lang.org/en/latest/tutorial/index.html#tutorial-index)

## Logical Programming

  - [ ] [Mercury](https://www.mercurylang.org/)
  - [ ] [TLA+](https://lamport.azurewebsites.net/tla/tla.html)

### [miniKanren](http://minikanren.org/)

  - [x] [The Reasoned Schemer](https://mitpress.mit.edu/books/reasoned-schemer)
  - [x] [microKanren: A Minimal Functional Core for Relational Programming](http://webyrd.net/scheme-2013/papers/HemannMuKanren2013.pdf)
  - [x] [Implement it in your favourite programming language](https://github.com/awalterschulze/gominikanren)

