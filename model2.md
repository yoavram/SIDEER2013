# Model 2

Following [@Hadany2002].

## The model

There are two haploid loci with alleles *a/A* and *b/B*.
The individual fitness landscape has two peaks and a valley between them, and the population occupies the lower peak [@Crow1990]:

1. The frequent type at the begining is *ab*.
1. The relative fitness of *ab* is 1
1. The single mutants *Ab* and *aB* have a lower fitness *1-s* 
1. The double mutant *AB* has a higher fitness *1+sH*

Forward and backward mutation rates in both loci are equal to $\mu$ and there is no recombination.

### Infinite population
We first consider an infinite population.
Neglecting terms of the order of $\mu^2$, we know that the frequency of each of the single mutatns is $p=\frac{\mu}{s}$. 

Neglecting terms in the order of $\mu^3$, we know that at the **mutation-selection balance** each generation a proportion of $2\frac{\mu}{s}\mu$ of the individuals are born *AB* because of a mutation in a single mutant and a proportion of $\mu^2$ of the individuals are born *AB* because of mutation in a wild type individual. 
Summing up, the proportion of individuals born *AB* born to parents who are not *AB* is:
$$
q_n = \mu^2 + 2p(1-s)\mu + O(\mu^3) = 
s^2 p^2 + 2p^2 (1-s)s + O(\mu^3) =
p^2(s^2 + 2s (1-s)) + O(\mu^3) =
p^2(s^2 + 2s - 2s^2) + O(\mu^3) \Rightarrow
q_n = (\frac{\mu}{s})^2(2s - s^2) + O(\mu^3)
$$
Denoting by *q* the total proportion of *AB* at equilibrium, we know that $q=q_n + q_0$, where $q_0$ is the frequency of *AB* born to *AB* parents.
The expected number of *AB* offspring born to a *AB* parent is given by
$$
\alpha = \frac{(1-\mu)^2 (1+Hs) + O(\mu^3)}{\bar{\omega}}
$$
The mean fitness is given by 
$$
\bar{\omega} = 1 - 2p - q + 2p(1-s) + q(1+Hs) =
 1-2p+q+2p-2sp+q+qHs = 
 1-2sp+qHs = 1 + O(\mu)
 $$
So
$$
\alpha = 1 + Hs + O(\mu)
$$
At equilibrium the proportion of *AB* individuals *q* is equal to the proportion of *AB* born to all individuals $q_0 + q_n$, and the proportion born to *AB* is equal to $q\alpha$:
$$
q_0 = q\alpha = (q_n + q_0)\alpha
$$
which gives us 
$$
q_o = \frac{q_n}{1-\alpha} \Rightarrow
q = \frac{q_n}{1-\alpha}
$$
Using the previous results we obtain:
$$
q = (\frac{\mu}{s})^2 \frac{2s - s^2}{-Hs} = 
(\frac{\mu}{s})^2 \frac{s - 2}{H} = 
$$

