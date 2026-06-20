A player throws three unbiased dice simultaneously. They notice that a sum of 11 can be formed by six combinations of faces (6:4:1, 6:3:2, 5:5:1, 5:4:2, 5:3:3, 4:4:3), and a sum of 12 can also be formed by six combinations (6:5:1, 6:4:2, 6:3:3, 5:5:2, 5:4:3, 4:4:4). The player concludes that rolling a 12 is just as likely as rolling an 11. Identify the fundamental conceptual fallacy in this reasoning, and calculate the true number of equiprobable outcomes favorable to each event


Solution

A Three dice result is an ordered 3-tuple


The prob of having 11 as the result :

First total outcomes is to ~~know~~ count how many ways each possible tuple can occur. (the first one, then second, then third)

ie 6:4:1 $\Rightarrow$

   6:3:2

   5:5:1

   5:4:2

   5:3:3

   4:4:3

for 3 distinct results in the tuple, there are $3!$ different ways of getting the constituents.

So we have gotten from 06 $(3! + 3!)$ for the first two

and for 2 distinct results numbers in tuple.

i.e 5:5:1 & 5:1:5 & 1:5:5

Gotten from $\frac{3!}{(\text{no of repeated numbers})} = \frac{3!}{2} = \frac{3 \times 2}{2}$

$$= 3$$

So

6:4:1 $\Rightarrow 3!$ ways

6:3:2 $\Rightarrow 3!$ ways

5:5:1 $\Rightarrow \frac{3!}{2}$ ways

5:4:2 $\Rightarrow 3!$ ways

5:3:3 $\Rightarrow \frac{3!}{2}$ ways

4:4:3 $\Rightarrow \frac{3!}{2}$ ways

So the sum of total ways

$$\Rightarrow 3! + 3! + \frac{3!}{2} + 3! + \frac{3!}{2} + \frac{3!}{2}$$

$$\Rightarrow 6 + 6 + 3 + 6 + 3 + 3$$

$$\Rightarrow 18 + 9 = \underline{\underline{27 \text{ ways}}}$$

Secondly, for the sum of 12, we have the following tuples


6:3:3 $\Rightarrow \frac{3!}{2}$

6:4:2 $\Rightarrow 3!$

5:5:2 $\Rightarrow \frac{3!}{2}$

5:4:3 $\Rightarrow 3!$

5:6:1 $\Rightarrow 3!$

4:4:4 $\Rightarrow \frac{3!}{3 \times 2}$

$$\Rightarrow \frac{3!}{2} + 3! + \frac{3!}{2} + 3! + 3! + 1$$

$$\Rightarrow 3 + 6 + 3 + 6 + 6 + 1$$

$$\Rightarrow 18 + 7 = \underline{\underline{25 \text{ ways}}}$$

Total Sample ~~ways~~ Space for 3 tuples is

$$= 6 \times 6 \times 6 = 216$$

So Pr. of getting 11 from 3 dice $= \frac{27}{216}$

Pr. of getting 12 from 3 dice $= \frac{25}{216}$

The true number of equiprobable outcomes & probability has been ~~shown~~ derived above

But the reason for the fallacy is the ~~correct~~ wrong counting of "favourable outcomes" or rather the ~~wrong~~ referral of what ~~was~~ ~~a~~ ~~"outcome"~~ a favourable outcome.

i.e the tuple 6:4:1 ~~result~~ gives the sum 11, but it doesn't ~~just~~ have these numbers resulting to the sum have more than one way of appearing. i.e 4:6:1 & not like the ~~number~~ tuple 4:4:4 that can only appear in one way (only 1 possible way).

