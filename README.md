# Little-o
I certify that I have listed all sources used to complete this exercise, including the use of any Large Language Models. All of the work is my own, except where stated otherwise. I am aware that plagiarism carries severe penalties and that if plagiarism is suspected, charges may be filed against me without prior notice.

I have used the help of chatGPT to help understand the definitions of big and 
little O and what it means, I worked it out on my own. I also had to look up the formal
definition of Big ) to use.

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

$f(n)\in O(g(n)) \iff \exists C>0, \exists n_0, \forall n\ge n_0: f(n) \le C g(n)$

 the little-o definition states that for every positive constant $c$, there exists 
 an $n_0$ such that $f(n) < c g(n)$ for all $n \ge n_0$. If we take c to equal  1,
 that means $f(n) < 1 g(n) = g(n),  \forall n\ge  n_0$
 This implies $f(n)\in O(g(n))$ keeping $C=1$ and $n_0$ the same. This is because 
 a less than is more strict than a less than or equal to and thus the less than or
 equal to will always be implied true under the conditions: $f(n)\in o(g(n))$ implies
that $f(n)\in O(g(n))$.
