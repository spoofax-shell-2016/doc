# Research questions

* What are REPLs?
  * How is the execution context/environment handled?
  * Comparison/feature matrix of some popular REPLs
    * Python and the IPython project
    * R
    * Lisp (Scheme, Racket)
    * Haskell
    * AutoCAD
* What is Literate Programming?
  * What are the key differences between the following literate programming solutions?
    * IPython/Jupyter notebooks
      More information: [Literate programming, RStudio, and IPython Notebook](https://biowize.wordpress.com/2015/03/13/literate-programming-rstudio-and-ipython-notebook/).
    * Swift playgrounds
      More information: [Swift Playgrounds](https://developer.apple.com/library/ios/recipes/Playground_Help/Chapters/AboutPlaygrounds.html).
    * Org-mode in Emacs (with Babel)
      Support for *tangling* source code within comments. See [The Org Manual](http://orgmode.org/manual/Working-with-source-code.html#Working-with-source-code) for more information.
  * How does Literate Programming relate to REPLs?
    Think about e.g. reevaluation of expressions (cascading results to later/earlier results).
* How and where does this project fit within Spoofax?
  * What is Spoofax?
  * How are language-specific commands handled?
  * How can a partial program (without entry point) be executed?
  * How can we integrate IDE specific features with generic REPL features?
    * What is the interaction with the editor views?
      For example jumping to definitions when clicking on types or function names.

