
**24/06/2026**

**6) Easy Conceptual:** Suppose you are choosing an ordered sample of size $r$ from a population of $n$ distinct objects. State the formulas for the total number of distinct ordered samples under two conditions: (a) Sampling with replacement, and (b) Sampling without replacement.

$$\underline{\text{Soln}}$$

For example, say we want to know the number of ways we can get **3 items** arranged from **6 total**.

$$\text{We have } \overset{\text{1st}}{6} \times \overset{\text{2nd}}{5} \times \overset{\text{3rd}}{4}$$

$$= 6! / 3! = \frac{6!}{(6-3)!} = \frac{n!}{(n-r)!}$$

$$= {}^n P_r = \text{permutation formula.}$$

**(a)** $\rightarrow$ Which is the total number of distinct ordered samples under the conditions

$\rightarrow$ Sampling without replacement.

> If Order didn't matter, then we reduce the duplicate counting of unordered list by dividing by $r!$ (the number of ways the list can be rearranged - for distinct items)
> 
> $$\text{i.e. } \frac{n!}{r!(n-r)!} = {}^n C_r = \binom{n}{r}$$

**(b)** ...Sampling with replacement

$$\rightarrow 6 \times 6 \times 6 = 6^3 = 216$$

$$$$
$$\text{but here } = n_1 \times n_2 \times \dots \times n_r = n^r$$
