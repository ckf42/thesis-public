# Self-similar Behavior of Boltzmann Equation under Shearing Effect 

This repo contains my thesis. Not sure if anyone may want to read this, but this may serve as a thesis template for other graduate students.

## Build

This thesis should be compiled with `XeLaTeX` and `biber`. If you have [TeXStudio](https://www.texstudio.org/), just press `Build & View` and it should generate the pdf (assuming you have all required packages installed).

## Commentary

### Section 2

Personally, I do not like this section. I will not give any more comment on this section.

### Section 3

I owe this part to the help from Professor Wang, who kindly shared his insight and ideas. Without his help, I would not be able to finish this section, let alone the results that build on this part.

### Section 4

In hindsight, this part is probably influenced by [Bassetti, Ladelli, and Matthes](https://doi.org/10.1214/ejp.v20-3531) (and to a *much* lesser degree, [Imbert, Silvestre, and Villani](https://arxiv.org/abs/2409.01183)), who consider constant function on the unit sphere, although I was (re-)reading a paper by Bobylev (forgot which one) when I came up with the idea.

Nevertheless, there are still many problems I was not able to solve/address, including
* why is the solution to the recurrence equation $R(n, i, j) = (1 - \frac{2 j}{n}) R(n - 1, i - 1, j) + \frac{2 j}{n} (1 + \frac{d - 1}{n - 1}) R(n - 2, i - 1, j - 1)$ on $0 \leq i, j \leq n / 2$ and $R(n, i, 0) = R(n, 0, j) = 1$ given by $R(n, i, j) = {}_3F_2(\frac{d - 1}{2}, -i, -j; -\frac{n - 1}{2}, -\frac{n}{2}; 1)$?
* are all matrices $S_n$ defined as $(S_n)_{ij} = \frac{n!}{j! (n - 2 j)! 2^j} R(n, i, j)$ always invertible? If so, how to compute the inverse (efficiently)?
* what is the most natural condition needed to have the argument work with the integral metric?
* however superficial it is, why do we see a connection with stable distributions, and why *now*?
* (if Blaschke-Levy condition is proven) why is it not needed for constant kernel in $\omega$ representation?

