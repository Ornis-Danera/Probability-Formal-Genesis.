

9 Easy Conceptual. When Partitioning a population of $n$ elements into $k$ subpopulations of sizes $n_1, n_2, n_3 \dots n_k$, what algebraic condition must the subpopulation sizes satisfy, and what is the formula (multinomial coefficient) for the number of distinct ways to achieve this Partition.




09/07/2026

Soln

(25)

Any set of ~~$r$ number~~ $\overset{\text{Subset}}{r\text{ elements}}$ chosen from a population of $n$ elements ($\overset{\text{Super set}}{\text{without regard}}$ for order (distinct order doesn't matter) is called a Subpopulation of size '$r$' of the original population.

We saw with example on Pg 6 that if we are to make 3 choices from 6 options, there are $6 \times 5 \times 4 \ \mathbf{\equiv} \ \frac{6!}{(6-3)!}$ ways to do that

& we also noted that each set from that number has $3!$ ways it can appear i.e

$$\left. \begin{matrix} \text{A B C} \\ \text{A C B} \\ \text{B A C} \\ \text{B C A} \\ \text{C A B} \\ \text{C B A} \end{matrix} \right\} \text{A, B, C}$$

and so to just get one unique set, we divide the total "distinct" number of ways of ~~choosing~~ choosing 3 from 6 by $3!$ $\ = \ \frac{6!}{(6-3)!} \times \frac{1}{3!} \ = \ \frac{6!}{3!(6-3)!}$ i.e

$$\left[ \begin{align*} &\text{i.e one set can appear } 3! \text{ times} \\ &\text{i.e } \text{ABC} \rightarrow 3! \text{ times}, \quad \text{EDP, } \ 3! \text{ times } \dots \\ &\text{so we factor out } 3! \\ &\quad (\text{ABC, } \ \text{EDP} \dots) \ 3! \quad \text{and divide by } 3! \end{align*} \right]$$

that $3!$ to get the actual ~~number of~~ set of elements from a population of $n$ elements without regard for order. ~~In the~~ In this case, 20 i.e ABC and EDP and $\dots$

Our maths tells us $\ = \ \frac{6!}{3!(6-3)!} \ = \ \frac{6 \times 5 \times 4 \times \cancel{3!}}{3! \ \cancel{3!}} = 20$



(26)

~~ABCEDP~~ $\quad$ ABC $\quad$ ABE $\quad$ ABD $\quad$ (ABCDEP)

~~ABCE~~ $\quad$ ~~AED~~ $\quad$ ~~ABD~~

$\qquad \qquad$ APD

~~A B C~~ $\quad$ A B E $\quad$ A BD $\quad$ ~~A B P~~

~~B C E~~ $\quad$ ~~B C D~~ $\quad$ ~~B C P~~ $\quad$ B C A

A B C $\quad$ ~~B C E~~ $\quad$ C E

A B E $\quad$ ~~B C D~~

~~A B D~~ $\quad$ B C P

~~A B P~~ $\quad$ ~~B C A~~

|**Starting with A**|**Starting with B without A**|**Starting with C without A or B**|
|---|---|---|
|A B C $\quad$ ~~8~~|B C D|C D E|
|A B D|B C E|C D P|
|A B E|B C P|C E P|
|A B P|B D E|3 ways|
|A C D|B D P||
|A C E|B E P|**Starting with D** **without A B or C**|
|A C P|6 ways|D E P|
|A D E||1 way|
|A D P|||
|A E P|||
|$\mathbf{\Rightarrow}$ 10 ways|$\mathbf{=}$ 20 ways||

That ABC could be arranged in 6 ways (as shown in Pg 6) same as the rest i.e ABD, ABE $\dots$

The proof is what we have indirectly/directly shown:

$\mathbf{\Rightarrow}$ If order mattered, then each of the elements above would have to be account for the distinct/different arrangements it could take.

So we have $\frac{6!}{3!(6-3)!}$ ~~multiplied by $3!$ to~~



(27)

~~give us that. But since we are looking~~

~~give us that. But since we are looking~~

**OR**

So the total count accounting for order is $\frac{6 \times 5 \times 4}{1} = \frac{6!}{(6-3)!} = n$

but to reduce the counting ~~by~~ removing "duplicates"/only accounting for the specific constituents of a set and not its arrangement we divide by the total number of ways we can do that to just get "unordered" count

$$\frac{6!}{(6-3)!} \div 3! \ = \ \frac{n!}{r!(n-r)!} \ = \ \frac{n(n-1)\dots(n-r+1)}{r!}$$

$$\text{or}$$

$$\ = \ \frac{6 \times 5 \times 4}{3!} \ = \ \frac{n(n-1)\dots(n-r+1)}{r!} \ = \ \frac{n!}{(n-r)!} \times \frac{1}{r!}$$

The above is also called a binomial coefficient often represented as $\begin{pmatrix} n \\ r \end{pmatrix}$ instead of $C_r^n$

Where $C_r^n$ is ~~mostly represented to refect~~ called the number of combination of $n$ thing taken $r$ at a time (or only $r$ things are taken without regard for order).

#### **Theorem 1:4**

Given a population of $n$ elements, let/where $(n_1, n_2, \dots, n_k)$ ~~be~~ all are positive numbers and that $n_1 + n_2 + \dots + n_k = n$,

Then there are $N = \frac{n!}{n_1! n_2! \dots n_k!}$ ways of partitioning $n$ elements into $K$ subpopulations of sizes $n_1, n_2, \dots \text{ or } n_k$ respectively.



Proof:

The order of subpopulations matters.

ie $n_1 = 2, \quad n_2 = 3, \dots, n_k$ is not same as $n_1 = 4, \quad n_2 = 2, \dots, n_k$.

The two above represent different partitions.

Note for this case the elements order for $n_1$ or any doesn't matter for now.

So for $n_1 = 2$, there are ~~$n_1$~~ $C_{n_1}^n$ ways of ~~arranging the~~ selecting $n_1$ elements from $n$. i.e $N_1 = C_{n_1}^n$

And that leaves us with $n - n_1$ elem

So for $n_2 = 3$, there are $C_{n_2}^{n-n_1}$ ways of selecting $n_2$ elements from what was left before. i.e $N_2 = C_{n_2}^{n-n_1}$

And that leaves us with ~~$n-n_1-n_2$~~

So for $n_3 = \text{say } 4$, there are $\overset{\swarrow \text{not important term}}{C_{n_3}^{n-n_1-n_2}}$ way of selecting $n_3$ elements from what was left before i.e $N_3 = C_{n_3}^{n-n_1-n_2}$

And that leaves us with $n - n_1 - n_2 - n_3$ elements and on and on on the last set of elements.

$$N_{K-2+1} = C_{n_{K-2+1}}^{n-n_1-\dots-n_{K-2}}$$

where $K-1$ is taken to be the last $n$th set.

$$N_{K-1} = C_{n_{K-1}}^{n-n_1-\dots-n_{K-2}}$$

So we can write that we have

$$\mathbf{N_1 \cdot N_2 \cdot N_3 \cdot N_{K-1}}$$

### **[Page 6]**

$$n - n_1 - n_2$$

$\begin{matrix} K-1=3 \\ K=4 \end{matrix} \quad N_1 \cdot N_2 \cdot N_3 \dots N_{K-1}$ total ways of forming $n_1, n_2, n_3 \dots n_{K-1}$ subpopulations or better stated (precisely),

$\mathbf{N} \rightarrow$ distinct ways of partitioning the given population $n$ into the indicated $K$ subpopulations.

$$\begin{align*} &\text{Note } \quad \cancel{\text{But}} \\ &N_1 \cdot N_2 \dots N_{K-1} \\ &= C_{n_1}^n \cdot C_{n_2}^{n-n_1} \dots C_{n_{K-1}}^{n-\dots-n_{K-2}} \\ \\ &= \frac{n!}{n_1!(n-n_1)!} \cdot \frac{(n-n_1)!}{n_2!(n-n_1-n_2)!} \cdot \frac{(n-n_1-n_2)!}{n_3!(n-n_1-n_2-n_3)!} \\ &\qquad \dots \frac{(n-n_1-\dots-n_{K-2})!}{(n_{K-1})!(n-n_1-\dots-n_{K-2}-n_{K-1})!} \\ \\ &= \frac{n!}{n_1!\cancel{(n-n_1)!}} \cdot \frac{\cancel{(n-n_1)!}}{n_2!\cancel{(n-n_1-n_2)!}} \dots \frac{\cancel{(n-n_1-\dots-n_{K-2})!}}{n_K! \ (n_K-1)!} \\ \\ &= \frac{n!}{n_1!} \times \frac{1}{n_2!} \times \frac{1}{n_3!} \dots \end{align*}$$

to show $n - n_1 \dots n_{K-2} - n_{K-1} \equiv n_K$ ~~ways~~

recall, $n_1 + n_2 + \dots + n_K = n$

subtracting $\mathbf{\swarrow}$ from L.H.S & R.H.S of $n_1 + n_2 + \dots + n_{K-1} \rightarrow \text{arbitrary}$

$$\begin{align*} \mathbf{\Rightarrow} \quad &n_K = n - (n_1 + n_2 + \dots + n_{K-1}) \\ &n_K = n - n_1 - n_2 \dots - n_{K-1} \end{align*}$$

$$\text{Shown!}$$

$$\text{So the last term} = \frac{(n - n_1 - \dots - n_{K-2})!}{(n_{K-1})! n_K!}$$

~~So the~~ The last term's numerator actually cancels out with a $\overset{\text{from}}{\text{term}}$ from the preceding denominator, leaving us with



$$\frac{n!}{n_1! n_2!} \dots \frac{1}{(n_{K-1})! n_K!}$$

$$= \frac{n!}{n_1! n_2! \dots n_k!}$$

Note: Theorem 1.3 is what we were dancing for on pg 25 - 26 - 27

$\rightarrow$ A population of $n$ elements has precisely $C_r^n = \frac{n!}{r!(n-r)!}$ subpopulations size $r \le n$.

And Theorem 1:4 on Pg 27 collapses to Theorem 1.3 if $K=2$

i.e $\frac{n!}{n_1! n_2!}$ where $\overset{\text{assumed}}{n_1 \text{ is now } r}$

$$\begin{align*} &\qquad \qquad n_2 = n - n_1 = n - r \\ &= \frac{n!}{r!(n-r)!} \end{align*}$$

$$\mathbf{N = \frac{n!}{n_1! n_2! n_3! \dots n_K!}} \quad \text{is called } \mathbf{\star}$$

multinomial coefficients

& recall $\frac{n!}{r!(n-r)!}$ is called generalized binomial coefficient



So now that I have read well Pg 7 & 8 of textbook, I can answer question 9

Soln

Algebraic Condition: $\mathbf{\equiv n_1 + n_2 + \dots + n_k = n}$

Multinomial Coefficient $\mathbf{\Rightarrow N = \frac{n!}{n_1! n_2! n_3! \dots n_k!}}$
