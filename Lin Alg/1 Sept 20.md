# Vector Space

### Linear Span

---



#### Definition 1.1

Let $V$ define a vector space.

If $x_1, x_2, x_3, .., x_n \in V$ then a linear combination is  
$$
c_1 x_1 +c_2 x_2 + .. + c_n x_n, c_i \in F
$$


Example let $V = \real (\real)$. Then elements are $1, 2, 3, 4, ..$

However, $1+2+3+4+..$ is not a linear combination. 



#### Definition 1.2

Again, let $V(F)$ be a vector space over the field $F$ then $S \subset V$ .
$$
LS(S) = \text{set of all possible linear combination of $S$}
$$
This also means $LS(S) \subset V$

---

#### Question 1.1

$V(F), |F| = 3, S \subset V, S = \{x_1, x_2\}, |LS(S)| = ? $

$|LS(S)| \leq  9$ because if $z \in LS(S)$ then $z = c_1 x_1 + c_2 x_2 $ for $c_1,c_2 \in F$

If $S$ is not $LD$ then $|LS(S)|=9$

#### Question 1.2

$|F| = 5, |S| = 3, |LS(S)|=?$

$LS(S) \leq 5^3$

---

### Linear Dependence

---

#### Definition 2.1

$V(F)$

$x_1, .., x_n \in V$ then they are called LD if there exists $c1, c2, .., c_n \in F$ and all non-zero st 
$$
c_1 x_1 + ... + c_n x_n = 0
$$
Then the set of $x_i$ is linearly dependent.



A set $S \subset V$ is either $LD$ or $LI$

---

#### Theorem 2.1

$V(F)$

Let $S = {x_1, x_2, ..., x_n} \in V$

then $S$ is $LD$ $\iff$ $\exists$ $ x_k \in S $ st
$$
x_k = c_1 x_1 + c_2 x_2 + .. + c_{k-1} x_{k-1} + c_{k+1} x_{k+1} + .. + c_n x_n
$$

##### Proof

$S$ is $LD$ $\iff$ $\exists$ $c_1, c_2, .., c_n \in F$ all not zero st $c_1 x_1 + .. + c_n x_n = 0 $

Just rearrange any non zero $c_k$ term and solve.

---

#### Question 2.1

$V(F)$, $|F| = 3$, $|S| = 2$, $S$ is $LD$

----

#### Theorem 2.2

$V(F)$

Let $S = {x_1, x_2, ..., x_n} \in V, x_1 \neq0$

then $S$ is $LD$ $\iff$ $\exists$ $ k>1$ st
$$
x_k = c_1 x_1 + c_2 x_2 + .. + c_{k-1} x_{k-1} + c_{k+1} x_{k+1} + .. + c_n x_n
$$

##### Proof

$S$ is $LD$ 

Consider $S_1 = \{x_1\}, S_2 = \{x_1, x_2\}, ..., S_n = \{x_1, x_2, .., x_n\}$

Choose smallest $k$ st $S_k$ is $LD$. Then $S_{k-1}$ is $LI$. 

Since $S_k$ is $LD$ $\exists c_1, c_2, .., c_k \in F$ not all zero st.
$$
c_1 x_1 + ... + c_k x_k = 0
$$
In this $c_k \neq 0$ because if it did then $S_{k-1}$ would be $LD$ which contradicts our assumption of $k$ being smallest such that $S_{k}$ is $LD$. 

Since $c_k \neq 0$ 
$$
x_k = -\frac{c_1}{c_n}x_1 -\frac{c_2}{c_k}x_2 .. -\frac{c_{k-1}}{c_k}x_{k-1}
$$

##### Example

$S = \{(1,0,0), (0,1,0),(2,2,0)\}$ is $LD$ because $x_3 = 2(x_1 + x_2)$

---

#### Theorem 2.3

$V(F)$

$S \subset V$ is LI

Then a subset $S' \subset S$ is also $LI$

##### Proof

Suppose $S'$ is $LD$. Then using theorem 2.1, $\exists x_m \in S_1$ st $x_m \in LS(S'-\{x_m\})$
$$
S' \subset S \implies S' - \{x_m\} \subset S-\{x_m\}
\\
\implies LS(S' -  \{x_m\}) \subset LS(S-\{x_m\})\\
\implies x_m \in LS(S-{x_m})
$$
This is contradiction as in conclusion this implies that if $x_m$ exists $S$ is $LD$ 

---

#### Theorem 2.4

$S \subset V$ and infinite set.

Then,

$S$ is linearly independent if all the finite subset of $S$ is $LI$.

---

#### Theorem 2.5

$S \subset V$ and $S$ is $LI$

$x \in V-s$

Then, $S \cup \{x\}$ is $LI \iff x \notin LS(S)$

##### Proof

If $S \cup \{x\}$ is  $LI$. Suppose $x \in LS(S)$. Then from definition 1.2
$$
x = c_1x_1 + .. + c_nx_n
$$
This gives contradiction.



If $x \notin LS(S)$.

 Suppose $S \cup \{x\}$ is  $LD$. Then
$$
\exists \text{ a finite set } S' \subset S\cup \{x\}\text{ which is $LD$}
$$
Also, $S'$ must contain $x$ because if it didn't $S'$ would be a subset of $S$ but $S$ is $LD$. This implies $x \in S'$

From Definition 2.1
$$
cx+c_1x_1+..+c_mx_m=0
$$
where $c \neq 0$ because $S$ is $LI$. This implies $x \in LS(S'-\{x\})$ and $x\in LS(S)$ which is a contradiction.

---

#### Theorem 2.6



Let $S \subseteq V$ and $|S|=n$. Let $T \subseteq LS(S)$ and $|T| = m$. Then $T$ is $LD$ if $m>n$

##### Proof

Lets $S=\{x_1,..,x_n\}$ and $T=\{u_1,..,u_n\}$. 

$T\subseteq LS(S)\implies u_i \in LS(S)$ for $i=1,2,...,m$

$u_i \in LS(S) \implies u_i = \sum_{j=1}^nA_{ij}x_j,(A_{ij}\in F) $



To show that when $m>n$. This equation has non-trivial soln
$$
c_1u_1+...+c_mu_m=0
$$
Solving
$$
c_1 u_1 +.. +c_m u_m =0 \\
\sum\limits_{i=1}^{i=m}c_i(\sum\limits_{j=1}^m A_{ij}x_j)=0\\
$$
Consider,
$$
\sum\limits_{i=1}^mC_i A_{ij}=0 \text{ for }j=1,...,n\\
(c_1,..,c_m)A_{m\times n} = (0,..,0)
$$
The vector $c_1,.,c_m$ must have non zero solution because rank of $A_{m\times n} \leq n$. N equations, M unknowns. 

---

#### Definition 2.2

Basis: $S \subseteq V$ is called basis of $V$ if $S$ is satisfying the following conidtions

1. $LS(S)=V$
2. $S$ must be $LI$

---

#### Theorem 2.7

$V(F)$ 

Let $B$ be basis for $V$. 

$B = \{x_1,..,x_n\}$

for each $x\in V \exists \text{ unique } c_1,c_2,...,c_n \in F$ st.

$X=\sum\limits_{i=1}^nc_i x_i$

##### Proof

Necessary for $LI$

---

#### Theorem 2.8

Every vector space has a basis.

Let $V(F)$ be a VS

$X = \{Y \subseteq V | V \text{ is } LI \} = \text{set of all $LI$ subsets of $V$}$

$(X, \subseteq )$ - partially ordered set.

Let $U$ be a chain of X

$W = \cup_{S\in U}S$

To show W is upperbound of V

1. $S \subseteq W$
2. $W \in X$ to Show $W$ is LI

If every finite subset of $W$ is $LI$, the $W$ is $LI$ 

$P_1 = \{x_1, ..,x_n\}\subseteq W$

$x_i \in s_{\alpha_i}$ $i=1,2,...,n$ $s_{\alpha_i} \in U $

Since $U$ is totally ordered set, there exists $\alpha_k$ st. 

$x_1, x_2,n .., x_n \in S_{\alpha_k} \implies P_1$ is $LI$

Any finite subset is $LI$.

Hence $W$ is $LI \implies W \in X \implies W$ is an upper bound of $U$. 