# 1. Natural Numbers





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

# 2. Integers

Subtraction is not defined on $\N$

So we extended the set to by introducing the negative of natural numbers.

And we get, 

$\Z = \{0,1,-1,2,-2,....\}$



$\Z$ forms a group under addition

$m+(-n)=$ $m-n$ if $m \geq n$

​                   $= -(m-n)$ else

$a-b=a+(-b)$

---

# 3. Rational Numbers

Multiplication on $\Z$  is defined

However, $\frac{m}{n}$ may not be in $\Z$. Enlarge $\Z$ by introducing elements of the form $\frac{m}{n}$. We get the set of rational numbers denoted by $\Q$. We can't introduce $\frac{m}{0}$



Denoted by $\Q$. Properties are 

1. $a+b\in \Q$ if $a,b\in\Q$
2. $(a+b)+c=a+(b+c)$ associative
3. $a+b=b+a$ commutative
4. $a+0=a \forall a \in Q$
5. For each $a \in \Q,\exists -a\in\Q$
6. Similar for multiplication


$\Q$ forms a field under addition and multiplication.

$\forall x,y \in \Q, x<y; \exists z \in \Q | x<z<y$

### Order Properties of \Q

To define $x<y$ .ie. $y-x$ is a positive rational number.

$\frac{m}{n}$ is positive if $m,n\in \N$ or both $(-m),(-n)\in N$

1) $a,b$ are positional then $a+b$ is postive

2. $a.b$ is also positive rational
3. Either $a$ or $-a$ is positive or $a==0$



We get a linear (or total) partial order on \Q by defining $a\leq b$ is $b-a$ is a positive rational number or $0$

Some special properties

1) $a<b \implies a+c<b+c$

2. $a<b, c>0 \implies ac <b c$

3. $a<b$ or $b>a$ or $a=b$

   

The field $\Q$ with the ordered relation.

### Density property of $\Q$



$\forall x,y \in \Q, x<y; \exists z \in \Q | x<z<y$

#### Proof

$$
x<y\\
x+x<x+y\\
x2<x+y\\
x<\frac{x+y}{2}\\
$$

Similarly $\frac{x+y}{2}<y$ 

So, $x<\frac{x+y}{2}<y$

Between any $x$ and $y$ there infinitely many rational number. So we say that $\Q$ is dense.

### Geometric Representation of Rational number



Number line. WIth origin and 1.



### Theorem 3.1

Let m be a positive natural number which is not a square. There does exist a $r\in \Q$ st. $r^2=m$

#### Proof

Suppose, if possible, $r=\frac{p}{q}$ where $gcd(p,q)=1$
$$
q^2r^2=p^2\\
q^2m=p^2
$$
$\exists $ a prime number $p_1$ st. the power of $p_1$ in$m$ is odd.
$$
p_1 | m \implies p_1 | p^2 \implies p_1 | p\\
p=p_1 m_1
mq^2=p_1^2m_1^2
$$
Case 1

Suppose if power of $p_1$ in $m$ is $1$, then 
$$
\frac{m}{p_1}q^2=p_1m_1^2\\
p_1|\frac{m}{P_1}q^2 \implies p_1|q^2\\
p_1 | q \text{ as $p_1$ is prime}\\
$$
$\implies gcd(p,q) \neq 1$ a contradiction.

SO $r$ is not rational.

Case 2.

If power of $p_1$ in $m$ is $>1$
$$
\frac{m}{p_1^2}=q^2=m_1^2
$$
and power of $p_1$ in $\frac{m}{p_1^2}>$0, so
$$
p_1|\frac{m}{p_1^2}q^2\\
p_1|m_1^2\\
p_1|m_1\\
m_1=p_1m_2\\
\frac{m}{p_1^2}q^2=p_1^2m_2^2\\
\frac{m}{p_1^4}q^2=m_2^2\\
...
\\
\frac{m}{p_1^{2s}}q^2=m_s^2 \text{ where the power of $p_1$ in $\frac{m}{p_1^{2s}}=1$}\\
\implies p_1|\frac{m}{p_1^{2s}} \implies p_1 | m_s^2\\
p_1 | m_s\\
m_s = p_1m_{s+1}
$$
So, $\frac{m}{p_1^{2s}p_1}q^2 = p_1m_{1+s}^2$where $\frac{m}{p_1^{2s}p_1}$ has no $p_1$ power.
$$
\implies p_1\cdot1q^2\implies p_1|q\\
\implies p1|gcd(p,q)
$$
So we have a contradiction 

Therefore, both cases give a contradiction. so $\sqrt{m}$ is a rational number



# 4. Real Numbers $\R$

The set of all rationals and irrationals in called real denoted by $\R$

### Axiomatic Definition of $\R$

$\R$ the set of all read number is a **complete ordered field**.



Algebraic structure of the real numbers gives short list (axioms) of basic properties of additions and multiplication.

In the terminology of abstract algebra, the set of real number forms a field with respect to addition and multiplication.



### Algebraic Axioms of $\R$

On the set of $\R$ two binary operations addition and multiplication satisfy the follower properties. 

A1. $a,b\in \R\implies a+b\in \R$ closure
A2. $a+b=b+a$ commutativity
A3. $(a+b)+c=a+(b+c)$ associativity
A4. $\exists 0 \in R$ st. $a+0=a \forall a\in \R$. existence of additive identity
A5. $\forall a\in \R \exists -a \in \R \ni a+(-a)=0$. Existence of additive inverse (negative element)

M1. $a,b \in R \implies a \cdot b \in \R$
M2. $a\cdot b = b\cdot a$
M3. $(a\cdot b)\cdot c=a\cdot (b\cdot c)$
M4. $\exists 1\in R, 1\neq 0 \ni a\cdot 1=a \forall a\in\R$ (existence of multiplicative identity (unit))
M5. $\forall a\neq0\in\R\exists a^{-1}\in\R \ni a\cdot a^{-1}=1$. Existence of mutliplicative inverse (reciprocal)

D4. $a\cdot (b+c) = a\cdot b+a\cdot c$ Distributive property of mutliplication over addition



