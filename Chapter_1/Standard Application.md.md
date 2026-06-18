Here is the verbatim transcription of the provided images, maintaining the layout, corrections, and structure of the handwritten text.





18/06/2026

Probability Theory. Mastery Examination: Basic Concepts

① [Standard Application]: A batch of 100 manufactured items is checked by an inspector, who randomly selects 10 items for examination. If none of the 10 items are defective, the batch is accepted. Calculate the exact probability that a batch containing exactly 10 defective items will be accepted, and express your intermediate steps using combinatorial notation:

Soln

The question triped me up at first. The phrase "Pr that a batch containing exactly 10 defective items will be accepted".

$$\rightarrow \begin{pmatrix} \text{different mathematical} \\ \text{objects.} \end{pmatrix}$$

The question is asking the Pr that in the selection of 10 out of 100, 10 ~~are~~ ~~defective.~~ ~~be accepted.~~ of picking 10 ~~defective~~ items. ~~\text{not}~~ exactly for that is the only way the batch ~~defective~~ bottles and is selected.

$$\therefore \text{Pr }(90 \text{ bottles "only" are good}) = \text{Pr}$$



Outcome is an ordered 10-tuple

(Sample Space)

Having assumed order, total sample space

$$100 \times 99 \times 98 \times 97 \times \dots \quad 91$$

$$= {}^{100}\text{P}_{10}$$

Tuple that fits description 
[good, good, ... good, good]



(Favorable outcomes)
~~Since~~ ~~we~~ ~~are~~ looking for the total number of ways of selecting 10 bottles from only 90 good ones. Because these are the number of ways that 10 defective are present but missed.

$$= 90 \times 89 \times \dots 81 = {}^{90}\text{P}_{10}$$

$$\therefore \frac{{}^{90}\text{P}_{10}}{{}^{100}\text{P}_{10}} = \frac{90 \times 89 \times \dots 81 \times 80 \dots}{80 \times 89 \dots} \div \frac{100 \times \dots 91 \times \dots}{90 \times 89 \dots}$$

$$= \frac{90 \times 89 \dots}{90 \times 89 \times 88 \times 87 \times \dots 81} \div 100 \times 99 \times \dots 91$$

The above is for when order matters.

$$= \frac{90 \times 89 \times 88 \times 87 \times 86 \times 85 \times 84 \times 83 \times 82 \times 81}{100 \times 99 \times 98 \times 97 \times 96 \times 95 \times 94 \times 93 \times 92 \times 91}$$

$$= \frac{90!}{(90-10)!} \div \frac{100!}{(100-10)!}$$

$$= \frac{90!}{80!} \times \frac{90!}{100!} = \frac{(90!)^2}{(80!)(100!)}$$

but for when order doesn't matter we ~~know~~ eliminate over counting "$r$" times by dividing by $r!$



i.e $\frac{90!}{10!(90-10)!} \div \frac{100!}{10!(90-10)!}$

Which is still same as before