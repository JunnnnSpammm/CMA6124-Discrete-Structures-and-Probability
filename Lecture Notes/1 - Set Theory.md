# Set Theory

## What you will learn in this lecture:
- Sets and its Structures
- Set Elements
- Cardinality of a Set
- Infinite Sets
- Equality of a Set
- Subset of a Set
- Power Set of a Set
- Operations on Sets
- Set Identities

## Definition of a Set
A set is an **unordered** collection of objects/elements/members.

Sets are usually denoted as follows
- S = {a, b, c}, set S is defined by listing its elements.
- T = {x | P(x)}, set T is defined by property of its element x, this is read as “x such that P(x)”

$x \in S$ informs us that object x is an element (a member) of the set S. This is read as “x is an element of S”
- N = {0, 1, 2, 3, 4, …} , so $3 \in N$
- T = {x | x is a letter of the English alphabets} , so $a \in T$

## Definition of a Set
Sets are unordered.

Thus {a, b, c} = {a, c, b} = {b, a, c} = {b, c, a} = {c, a, b} = {c, b, a}. All of those sets above are equal!

All elements are **distinct** (unequal); multiple listings make no difference! Suppose a = b, then T = {a, b, c} = {a, c} = {b, c} ={a, a, b, a, b, c, c, c, c}.

If x is NOT an object in a set, then we use the symbol, $\not\in$. 

x $\not\in$ S informs us that object x is NOT in S.

## Cardinality of a Set
**Cardinality:** is defined as the number of **distinct elements** in a set.

|M| refers to the cardinality of set M. These two lines are used to refer to cardinality.

If |T| = 0, then we also write T = $\emptyset$ or T = { }. These are known as **empty set** or **null set**

If |S| = A, where A is some number, then we say S is **finite** or countable. Otherwise, we say S is **infinite** or uncountable.

## Common Infinite Sets to Know
- Set of **natural** numbers, $N$ = {0, 1, 2, 3, 4, 5, …}, also known as counting number or nonnegative integer
- Set of **integers**, $Z$ = {…, −2, −1, 0, 1, 2, …}
- Set of **positive integers**, $Z^+$ = {1, 2, 3, …}
- Set of **negative integers**, $Z^-$ = {-1, -2, -3, …}
- Set of **rational** numbers, $Q$ = { $\frac{p}{q}$ | $p \in Z, q \in Z, q \neq 0$}, another name for rational numbers is fractions
- Set of **real** numbers, $R$ = {All real numbers} 

## Equality of a Set
Two sets are **equal** if and only if they have the same members. It does not matter how the set is defined or denoted!

## Subsets and Proper Subsets
A set **S** is said to be a **subset** of another set **T** if and only if every element of set **S** is contained in set **T**.

The notation for subset is $\subseteq$, $S \subseteq T$. **Note that: Subsets of set T includes the set itself. That is, T $\subseteq$ T**

A set **S** is said to be a **proper subset** of another set **T** if and only if set **S** is a subset of set **T** but set **S** is not equal to set **T**. The notation for proper subset is $\subset$, $S \subset T : S \subseteq T$ and $S \neq T$
**This means: A proper subset for set T is ALL subsets of set T EXCEPT the set itself.**

## Power Sets
A **power set** P(S) of a set S is the set of all subsets of S. P(S) = {x | $x \subseteq S$}

Example: If S = {a,b}, then P(S) = { $\emptyset$, {a}, {b}, {a,b}}.

Another notation for P(S) is $2^S$.

**Cardinality of a Power Set**
- If S is finite then |P(S)| = $2^{|S|}$.
- |P(N)| > |N|.

## The Universal Set
The idea of a “set of all sets” leads to logical difficulties.

Difficulties are avoided by always working within a local “universal set” which includes only those objects under consideration.

For example, when discussing arithmetic, it might be sufficient to work just with the numbers ..., -3, -2, -1, 0, 1, 2, 3, ...

Our universal set could then be taken as Z and other sets of interest, such as {x: x is prime}, are parts of Z.

The Universal set notation is $U$.

## Operations on Sets
- **Union:** $A \cup B$ = { $x \mid x \in A$ or $x \in B$}
- **Intersection:** $A \cap B$ = { $x \mid x \in A$ and $x \in B$}
- **Difference:** $A - B$ = { $x \mid x \in A$ and $x \notin B$}
- **Complement of $A$:** $\overline{A} = A^c = U - A$ where $U$ is the universal set
- **Symmetric difference of two sets $A$:**
  * $A \triangle B = (A - B) \cup (B - A)$
  * $A \triangle B = (A \cup B) - (A \cap B)$

## Summary
We have learnt the following concepts related to sets:
- Notation for sets,
- $\in$ relational operator,
- cardinality |S|, the empty set $\emptyset$ and infinite sets N, Z, Q, R,
- equal sets, subsets and proper subsets $=, \subseteq, \subset$,
- power sets P(S),
- set operations $\cup, \cap, \overline{}, S^c$
