## Topics in Cauchy Sequence

### Basics:

**Definition:** A sequence $\\{a_n\\}$ is called cauchy sequence iff $\forall \varepsilon>0$ $\exists N \in \mathbb{N}$ such that if $m,n \geq N$ then $|a_n-a_m|< \varepsilon$.

**Example:** $\\{\frac{1}{n}\\}_{n\geq 1}$ is cauchy sequence.

**Proof:** Take $\varepsilon >0$ and we need to find $N \in \mathbb{N}$. Now, for $|\frac{1}{n}-\frac{1}{m}|<\varepsilon$, we need the $N$. But see that $|\frac{1}{n}-\frac{1}{m}|<|\frac{1}{n}|+|\frac{1}{m}|<\frac{2}{n}$(wlog say $m>n$). So, if we take $\frac{2}{n}<\varepsilon \Rightarrow n \geq \lceil \frac{2}{\varepsilon} \rceil=N$ we are through. And as $m>n \geq N$ we have $m,n \geq N$.

---

### Properties:
1. If a subsequence of a cauchy sequence is convergent to some point $\ell$ then the whole sequence is going to converge to that point $\ell$.

**Proof:** Let a cauchy sequence be $\{a_n\}$ and its subsequence be $\{a_{n_k}\}$. Now, let $\{a_{n_k}\} \rightarrow \ell$. Then by definition, $\forall \varepsilon >0$ $\exists N_1 \in \mathbb{N}$ such that $k\geq N_1 \Rightarrow$ $|a_{n_k}-\ell|<\varepsilon/2$. Now, as the sequence is cauchy, then we have the following: \
$\exists N_2$ such that $n,m \geq N_2 \Rightarrow |a_m-a_n|<\varepsilon/2 $. Now, there is some $N_3$ such that if $k \geq N_1$ then $n_k \geq N_3$. Then take $N= max\{N_3,N_2\}$ we get, $n_k,n \geq N\Rightarrow $ $|a_{n_k}-a_n|<\varepsilon/2$ and $|a_{n_k}-\ell|<\varepsilon/2 $, adding this two we get, $n \geq N_2 \Rightarrow $ $|a_n-\ell|<\varepsilon$.

2. Every cauchy sequence is bounded.

**Proof:** Proof is done [here](https://atrajit-sarkar.github.io/Real-Analysis/#cauchy-sequences).

3. **General Sequence Property:** Every bounded sequence in $\mathbb{R}$ must have a covergent subsequence. 

**Proof:** This proof is tricky and this is called **Bolzano–Weierstrass theorem** Theorem. You can read proof from [here](https://en.wikipedia.org/wiki/Bolzano%E2%80%93Weierstrass_theorem). 

---

## Conclusion

### Theorem:
Every cauchy sequence in $\mathbb{R}$ is covergent.

**Proof:** We know from Property 2 that every cauchy sequence is bounded. And also from property 3 we see that every bounded sequence in $\mathbb{R}$ must have a covergent subsequence. Then together we get that the cauchy sequence in $\mathbb{R}$ must have a cobergent subsequence. Say, the subsequence is coverging to $\ell$. then we get from property 1 that the whole cauchy dequence should converge to the point $\ell$, and that is the proof that every cauchy sequence in $\mathbb{R}$ is covergent. 

**Note:** You might get different proofs of the above fact using contradiction, but those proofs have flaws. Try to find the flaws and discuss with me. If you find difficulity we will discuss it later in class.

---
## Happy Reading...............
