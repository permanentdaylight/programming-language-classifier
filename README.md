Getting a corpus of programming languages
Option 1: Get code from the Computer Language Benchmarks Game. You can download their code directly. In the downloaded archive under benchmarksgame/bench, you'll find many directories with short programs in them. Using the file extensions of these files, you should be able to find out what programming language they are.

Option 2: Scrape code from Rosetta Code. You will need to figure out how to scrape HTML and parse it. BeautifulSoup is your best bet for doing that.

Option 3: Get code from GitHub somehow. The specifics of this are left up to you.

You are allowed to use other code samples as well.

For your sanity, you only have to worry about the following languages:

C (.gcc, .c)
C#
Common Lisp (.sbcl)
Clojure
Haskell
Java
JavaScript
OCaml
Perl
PHP (.hack, .php)
Python
Ruby (.jruby, .yarv)
Scala
Scheme (.racket)
Feel more than free to add others! (like C++, Elixir, Julia, Elm, HTML, CSS, SQL, etc)

Classifying new snippets
Using your corpus, you should extract features for your classifier. Use whatever classifier engine that works best for you and that you can explain how it works. Either using an existing Transformer or one you've written. Be sure you can explain at a high-level how your Transfomer works.

Write a classifier function that takes a string of code and returns a guess for the language the code was written in. It is recommended you also have a method that returns the snippet's percentage chance for each language in a dict.
