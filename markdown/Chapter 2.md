# Chapter 2: Information Measures

April 18, 2020



## 2.1. Independence and Markov Chain

#### > Notations

- $X$: discrete rarndom variable taking values in $\mathcal{X}$.

- $\left\{p_{X}(x)\right\}$: probability distribution of $X$.

- $\mathcal{S}_{X}$: ==support== of $X$, i.e., $\left\{x \in \mathcal{X} | p_{X}(x)>0\right\}$

  - if $\mathcal{S}_{X} = \mathcal{X}$, we say that $p$ is **strictly positive**.

    

#### > Proposition 2.4: Conditional Independence

![image-20200418210219728](/Users/ziyuye/Desktop/Information Theory/images/2-1-1.png)

The above is the graph showing how $X$, $Y$ and $Z$ are related, for the case: $X \perp Z | Y$, in other words, $X$ is independent of $Z \perp Y$.

- $p(x,y,z)=p(x)p(y|x)p(z|y)$
- $p(x,y,z)=p(x,y)p(z|y)$
- $p(x,y,z)=\frac{p(x, y) p(y, z)}{p(y)}$
- Think of passing $X$ through the channel $p(y|x)$ to obtain $Y$, and pass $Y$ through the channel $p(z|y)$ to oabtain $Z$.

Think it alternatively:

- if $X \perp Z | Y$:  ==$p(x,y,z)=p(x,y)p(z|y)$==
- if not $X \perp Z | Y$:  ==$p(x,y,z)=p(x,y)p(z|x,y)$==



#### > Proposition 2.5: Necessary and Sufficient Condition of Condional Independence

> ==$X \perp Z | Y$ if and only if $p(x,y,z)=f(x,y)g(z,y)$.==

Note:

- $f(\cdot)$ and $g(\cdot)$ are not necessarily probability functions. They just need to be functions that depends only on the specified variables.

  