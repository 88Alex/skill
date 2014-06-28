Skill- A New Programming Language
=================================

Skill is a new programming language unlike any other in existence.
What makes Skill new is its combination of multiple paradigms:
object-oriented, functional, and imperative.

How about an example?
---------------------

```
(defclass A {
	(defmember @private int x)
	(defmember @public int y)
	(defmethod @public (foo a b)
		(print a " & " b)
	)
} )
(deffunc (factorial n)
	(if (eq? n 1) 1 (factorial (- n 1)))
)
(defproc @int (factorial2 @int n) {
	(if (n == 1) { -- both prefix and infix? why not?
		1
	} )
	(defvar int result 1)
	(foreach i (2..n) {
		(result *= i)
	}
	result
} )
(defvar A a (new A))
(a foo 3 5)
(a.foo 4 6) -- both styles work
(print (factorial 5))
(print (factorial2 5))
(exit 0)
```
