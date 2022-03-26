# Choice and Preferences

## Basic mathematical objects

<br>

A finite set $X$ of **outcomes**

A finite set $\mathcal{X} = \{ S : S \in 2^{X} - \{ \empty \} \}$

<br>

## Binary relations over $X$

<br>

For any $x, y \in X$, we have three possible relations:

1. [Preference](): 
   
$$
xRy := \text{x is at least as good as y}
$$

2. [Strict Preference](): asymmetric

$$
xPy := xRy \text{ and } \neg yRx
$$

3. [Indifference](): symmetric

$$ 
xIy := xRy \text{ and } yRx
$$

## Derived mathematical objects

<br>

From $R$, we can construct the [**Maximal Set**]() $M$, defined as follows:

* For $S \in \mathcal{X}$, and a relation $R$

$$M( R, S ) = \{ x \in S : \forall y \in S, xRy \}$$

    I.e.: the maximal set contains the alternatives that beats EVERY other alternatives in the set

## Properties of $R, P, \text{ and } I$

<br>

1. [Reflexivity](): for all $x \in X$

$$
xRx
$$

2. [Completeness](): for all $x, y \in X$ s.t. $x \neq y$

$$
xRy \text{ or } yRx
$$

        inclusive or

3. [Transitive](): for any $x, y, z \in X$

$$
xRy \text{ and } yRz \rightarrow xRz
$$

    this property also holds for Strict Preferences and Indifference

A consequence of transitivity is that, for any $x, y, z \in X$:

$$
xRy \text{ and } yPz \rightarrow xPz\\

xPy \text{ and } yRz \rightarrow xPz\\
$$

    i.e.: transitivity still holds for combinations of Strict and Standard preference relations

4. [Quasi-Transitive](): for any $x, y, z \in X$

$$
xPy \text{ and } yPz \rightarrow xPz
$$

5. [Acyclic](): for all $\{ x, y, z, ..., u, v \} \in X$

$$
xPy \text{ and } yPz, ..., \text{ and } uPv \rightarrow xRv
$$

    notice that the implied relation is not the Strict Preference, but just the Standard Preference relation, even though we assume Strict Preferences

6. [Weak Order](): a **reflexive, complete, and transitive** binary relation. If we have an weak order $R$ over a set $S \in \mathcal{X}$, for any $S$

$$
M( R, S ) \neq \empty 
$$

## Theorems

[Theorem 1.1]( ): let $R$ be reflexive and complete, then, for all $S \in \mathcal{X}$

$$
M( R, S ) \neq \empty \iff R \text{ is acyclic}
$$