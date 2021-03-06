[Exercise 9.23](ex_23/)

Suppose a knowledge base contains just the following first-order Horn
clauses:

$$
Ancestor(Mother(x),x)
$$
$$
Ancestor(x,y) \land Ancestor(y,z) \implies Ancestor(x,z)
$$

Consider a forward chaining algorithm that, on the $j$th iteration,
terminates if the KB contains a sentence that unifies with the query,
else adds to the KB every atomic sentence that can be inferred from the
sentences already in the KB after iteration $j-1$.

1.  For each of the following queries, say whether the algorithm
    will (1) give an answer (if so, write down that answer); or (2)
    terminate with no answer; or (3) never terminate.

    1.  $Ancestor(Mother(y),John)$

    2.  $Ancestor(Mother(Mother(y)),John)$

    3.  $Ancestor(Mother(Mother(Mother(y))),Mother(y))$

    4.  $Ancestor(Mother(John),Mother(Mother(John)))$

2.  Can a resolution algorithm prove the sentence
    $\lnot Ancestor(John,John)$ from the original knowledge base?
    Explain how, or why not.

3.  Suppose we add the assertion that $\lnot(Mother(x){{\,=\,}}x)$ and
    augment the resolution algorithm with inference rules for equality.
    Now what is the answer to (b)?

