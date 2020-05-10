				━━━━━━━━
				 README
				━━━━━━━━


Table of Contents
─────────────────

1 Build My Own Lisp
.. 1.1 Building
.. 1.2 Running
.. 1.3 Examples
.. 1.4 Progress


1 Build My Own Lisp
═══════════════════

  Learning C and building my own programming language with the book
  ["Build Your Own Lisp"].


  ["Build Your Own Lisp"] http://www.buildyourownlisp.com


1.1 Building
────────────

  Just run:
  ┌────
  │ make
  └────


1.2 Running
───────────

  After building type:
  ┌────
  │ ./lispy
  └────


1.3 Examples
────────────

  Arithmetic operations:
  ┌────
  │ lispy> + (* 2 (- 1 3) (/ 4 2)) 
  │ -8
  └────

  List functions:
  ┌────
  │ lispy> eval (head (tail (join {1 2} (list 3 4 5))))
  │ 2
  └────

  Variable functions:
  ┌────
  │ lispy> def {x z} 123 -321
  │ ()
  │ lispy> x
  │ 123
  │ lispy> y
  │ -321
  │ lispy> = {x} 1
  │ ()
  │ lispy> x
  │ 1
  └────

  Lambda functions:
  ┌────
  │ lispy> \ {x y} {+ x y}
  │ (\ {x y} {+ x y})
  └────

  Functions defenition:
  ┌────
  │ lispy> fun {curry f xs} {eval (join (list f) xs)}
  │ ()
  │ lispy> curry + {5 6 7}
  │ 18
  └────

  Comparison operations:
  ┌────
  │ lispy> > 3 1
  │ 1
  └────

  Logical operators:
  ┌────
  │ lispy> def {x y z} 1 2 3
  │ ()
  │ lispy> if (or (== x y) (>= z y)) {+ x y} {- x y}
  │ 3
  └────

  Get local environment:
  ┌────
  │ lispy> locals {}
  │ {{+ <builtin>} {- <builtin>} {* <builtin>} {/ <builtin>}
  │  {> <builtin>} {>= <builtin>} {< <builtin>} {<= <builtin>}
  │  {== <builtin>} {!= <builtin>} {if <builtin>} {or <builtin>} 
  │  {and <builtin>} {not <builtin>} {list <builtin>} {head <builtin>}
  │  {tail <builtin>} {eval <builtin>} {join <builtin>} {def <builtin>}
  │  {\ <builtin>} {fun <builtin>} {= <builtin>} {locals <builtin>}
  │  {exit <builtin>}}
  └────

  Strings, comments and file execution
  ┌────
  │ ./lispy hello.lspy
  │ "Hello World!"
  └────

  or

  ┌────
  │ lispy> load "hello.lspy"
  │ "Hello World!" 
  │ ()
  └────

  Standard library functions:
  ┌────
  │ lispy> map (\ {x} {+ x 10}) {5 2 11}
  │ {15 12 21}
  │ lispy> filter (\ {x} {> x 2}) {5 2 11 -7 8 1}
  │ {5 11 8}
  └────

  Exit function (or use `Ctrl+C'):
  ┌────
  │ lispy> exit {}
  └────


1.4 Progress
────────────

  • ☑ Chapter 1 • Introduction
  • ☑ Chapter 2 • Installation
  • ☑ Chapter 3 • Basics
  • ☑ Chapter 4 • An Interactive Prompt
  • ☑ Chapter 5 • Languages
  • ☑ Chapter 6 • Parsing
  • ☑ Chapter 7 • Evaluation
  • ☑ Chapter 8 • Error Handling
  • ☑ Chapter 9 • S-Expressions
  • ☑ Chapter 10 • Q-Expressions
  • ☑ Chapter 11 • Variables
  • ☑ Chapter 12 • Functions
  • ☑ Chapter 13 • Conditionals
  • ☑ Chapter 14 • Strings
  • ☑ Chapter 15 • Standard Library
  • ☑ Chapter 16 • Bonus Projects
  • 🚀 Work on improvements and new features…
