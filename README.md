# Little-o

In addition to the big-O, big-$\Omega$, and big-$\Theta$ notation that
we covered at the beginning of this class, a few other notations are sometimes
used in asymptotic analysis.  For example, "little-$o$" notation.

Prove (i.e.\ give a formal mathematical proof) that $f(n)\in o(g(n))$ implies
that $f(n)\in O(g(n))$.

Hint: The proof will be *very* short and *very* easy. You can start by
identifying the differences between the definitions of O and o.

I have started with the formal definition of $o$ below. Add your answer to this
markdown file. [This
page](https://docs.github.com/en/get-started/writing-on-github/working-with-advanced-formatting/writing-mathematical-expressions)
might help with the notation for mathematical expressions.

$f(n)\in o(g(n)) \iff \forall c>0, \exists n_0, \forall n\ge n_0: f(n) < c g(n)$

We need the definition of Big 0
$\n f(n)\in O(g(n)) \iff \exists C>0, \exists n_0, \forall n\ge n_0: f(n) \le C g(n)$

 the little-o definition states that for every positive constant $c$, there exists 
 an $n_0$ such that $f(n) < c g(n)$ for all $n > n_0$. If we take c to equal  1,
 that means $f(n) < 1 g(n) = g(n),  \forall n\ge  n_0$
 This implies the condition for $f(n)\in O(g(n))$
