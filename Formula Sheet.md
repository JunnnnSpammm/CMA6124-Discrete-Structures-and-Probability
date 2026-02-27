# Appendix A

## List of Rules of Inference

**ADD:** $p \Rightarrow (p \vee q)$

**SIMP:** $[p \wedge q] \Rightarrow p$

**CONJ:** $p \wedge q \Rightarrow (p \wedge q)$

**MP:** $[(p \rightarrow q) \wedge p] \Rightarrow q$

**MT:** $[(p \rightarrow q) \wedge (\neg q)] \Rightarrow \neg p$

**HS:** $[(p \rightarrow q) \wedge (q \rightarrow r)] \Rightarrow (p \rightarrow r)$

**DS:** $[(p \vee q) \wedge (\neg p)] \Rightarrow q$

**RES:** $[(p \vee q) \wedge (\neg p \vee r)] \Rightarrow (q \vee r)$

---

## List of Logical Equivalence Laws

* **Conversion of Implication:** $p \rightarrow q \Leftrightarrow \neg p \vee q$
* **Conversion of Equivalence:** $p \leftrightarrow q \Leftrightarrow (p \rightarrow q) \wedge (q \rightarrow p)$
* **Double Negation:** $\neg \neg p \Leftrightarrow p$
* **De Morgan:**
    * $\neg (p \wedge q) \Leftrightarrow (\neg p \vee \neg q)$
    * $\neg (p \vee q) \Leftrightarrow (\neg p \wedge \neg q)$
* **Domination:**
    * $p \wedge \mathbf{F} \Leftrightarrow \mathbf{F}$
    * $p \vee \mathbf{T} \Leftrightarrow \mathbf{T}$
* **Negation:**
    * $p \wedge \neg p \Leftrightarrow \mathbf{F}$
    * $p \vee \neg p \Leftrightarrow \mathbf{T}$
* **Identity:**
    * $p \wedge \mathbf{T} \Leftrightarrow p$
    * $p \vee \mathbf{F} \Leftrightarrow p$
* **Commutative:**
    * $p \wedge q \Leftrightarrow q \wedge p$
    * $p \vee q \Leftrightarrow q \vee p$
* **Idempotent:**
    * $p \vee p \Leftrightarrow p$
    * $p \wedge p \Leftrightarrow p$
* **Distributive:**
    * $p \wedge (q \vee r) \Leftrightarrow (p \wedge q) \vee (p \wedge r)$
    * $p \vee (q \wedge r) \Leftrightarrow (p \vee q) \wedge (p \vee r)$
* **Associative:**
    * $p \vee (q \vee r) \Leftrightarrow (p \vee q) \vee r \Leftrightarrow p \vee q \vee r$
    * $p \wedge (q \wedge r) \Leftrightarrow (p \wedge q) \wedge r \Leftrightarrow p \wedge q \wedge r$
* **Absorption:**
    * $p \vee (p \wedge q) \Leftrightarrow p$
    * $p \wedge (p \vee q) \Leftrightarrow p$
