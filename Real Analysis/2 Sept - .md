# Natural Numbers





$\mathrm{N}$ defines a set of natural numbers. It also has the operations $+, \cdot$

This set is also totally ordered.

---

### Theorem 1.1 Well Ordering Property

Every non-empty subset of $\N$ has a least element. This means if $S \subset \N, x \neq \phi$ then there is $m \in S$ st. $m\leq s \forall s \in S$

#### Proof

Let $k \in S$ . Let $T=\{s|s \leq k  \text{ and } s \in S \}$

There $T$ is a finite set, so $T$ has a least element $m$

##### Claim - $m$ is the least elt. of $S$

Suppose not, then there is $s_1\in S$ st. $s_1<m$

So, $s_1<m \leq k$, so $s_1\in T,$ and $s_1<m$ which contradicts that $m4 is the least elt of T

---

### Theorem 1.2 Principle of Induction

Let $P(n)$ be a statement involving a natural number $n$ 

1. $P(1)$ is true
2. $P(k+1)$ is true whenever $P(k)$ is true

Then $P(n)$ is true for all $n \in \N$



Equivalently, 



Let $S \subseteq \N$ st.

1. $1 \in S$
2. $k \in S \implies k+1 \in S$

Then, $S=N$



#### Proof

Suppose if possible $S \neq \N$

Let $T=N-S, T \neq \phi$

By Theorem 1.1, There is a least elt. $m$

Some $m>1$ as $1\in S$

As $m$ is least element of $T=S^c$ so $m-1\in S$

$\implies (m-1)+1\in S \implies m \in S$ which is a contradiction. So $S = \N$

---

# Integers

Subtraction is not defined on $\N$

So we extended the set to by introducing the negative of natural numbers.

And we get, 

$\Z = \{0,1,-1,2,-2,....\}$



$\Z$ forms a group under addition

$m+(-n)=$ $m-n$ if $m \geq n$

​                   $= -(m-n)$ else

$a-b=a+(-b)$

---

# Rational Numbers

Multiplication on $\Z$  is defined

However, $\frac{m}{n}$ may not be in $\Z$. Enlarge $\Z$ by introducing elements of the form $\frac{m}{n}$. We get the set of rational numbers denoted by $\Q$. We can't introduce $\frac{m}{0}$

