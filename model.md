# Model

We denote four genotypes: $AB$, $Ab$, $aB$, and $ab$.

We denote their frequencies as $f_{i,j}$, their fitness as $\omega_{i,j}$ and their mutation rates as $\mu_{i,j}$ for $i,j \in {A,a,B,b}$.

If $f=(f_{AB}, f_{Ab}, f_{aB}, f_{ab})$ is the frequency vector, then the mutation matrix $M$ is:

$$M=
\begin{array}{cccc}
(1-\mu_{A,B} \delta)^2 & (1-\mu_{A,b} \beta)\mu \beta & (1-\mu_{a,B} \beta)\mu_{a,B} \beta & \mu_{a,b}^2 \beta^2 \\\
(1-\mu_{A,B} \delta)\mu_{A,B} \delta & (1-\mu_{A,b})^2 + \mu^2 \beta \delta & \mu_{a,B}^2 \beta \delta & (1-\mu_{a,b} \beta)\mu_{a,b} \beta\\\
(1-\mu_{A,B} \delta)\mu \delta & \mu_{A,b}^2 \beta \delta & (1-\mu_{a,B})^2 + \mu_{a,B}^2 \beta \delta & (1-\mu_{a,b} \beta)\mu_{a,b} \beta \\\
\mu_{A,B}^2 \delta^2 & (1- \mu_{A,b} \beta)\mu_{A,b} \delta & (1- \mu_{a,B} \beta)\mu_{a,B} \delta & (1-\mu_{a,b} \beta)^2 \\\
\end{array} 
$$
where $\beta$ and $\delta$ are the probabilities that mutations are beneficial or deleterious, respectively ($\mu$ measures the probability that a fitness changing mutation occurred, so that $\beta+\delta=1$).

The selection matrix given a multpl