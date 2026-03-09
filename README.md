# possible journal to submit
1. Annals of Applied Probability
2. Journal of Functional Analysis




# Comments for next meeting:
1. we need a new notation for $M_{i,j}(f)$, as $M_{x_i,x_j}$ being used for marks in edge-marked Poisson process
7. Should we change "Remark 6.4" to a corollary?

8. subgraph count for non-integrable connection function

Let $W_s\subset\mathbb{R}^d$ be a convex set with volume $Vol(W_s)=s$.
Let $f:\mathbb{R}^d\to[0,1]$ be a measurable radial function with polynomial decay, i.e., $f(x)=\bar{f}(|x|)\sim |x|^{-\alpha}$. Suppose $\alpha\in(0,d)$, that is $f$ is non-integrable on $\mathbb{R}^d$. 
There exist constants $r_1>0$ and $c>0$ such that 
$$
\operatorname*{ess~inf}_{r\le r_1}\bar{\varphi}(r)\ge c.
$$
Suppose $F$ is a connected graph with $k\ge2$ edges, and denote $E(F)$ the edge set of graph $F$.
Looking for low bound of 
$$
I_k(s):=\int_{W_s^{k}}\prod_{\{i,j\}\in E(F)}f(x_i-x_j)\mathrm{d}x_1\cdots\mathrm{d}x_k
$$

Assume that for each $x_1 \in W_s$,
$$
\int_{W_s^{k-1}} \prod_{1 \le i < j \le k} f(x_i - x_j)\, \mathrm{d}x_2 \cdots \mathrm{d}x_k > 0.
$$
This assumption ensures only that $$ I_k(s) > 0 $$, but it gives no quantitative lower bound
on the order of growth of $I_k(s)$ in $s$.

Indeed, one may construct a radial $f$ with the same polynomial tail
but supported on a union of exponentially thin spherical shells, for instance:
$$
f(r) = r^{-\alpha} \mathbf{1}_{\bigcup_{m \ge 1} (m,\, m + e^{-m^2})}(r).
$$
For such a function, the above integral remains positive,
yet the measure of configurations where all pairwise distances lie within these shells
can decay faster than any power of $s$.
Hence, positivity of the inner integral does *not* suffice to yield a polynomial lower bound.


------updated on 2nd Dec, 2025---
if we can find a global infimum for the connection function, i.e., 
$$
\inf_{x,y\in\Gamma_s}\varphi(x-y)\ge c_1 s^{-\alpha/d},
$$
then the optimatization strategy will be in the same favor as in my work with Nicolas. We might need some balanced condition to determine the leading order of variance. 

-------updated on 5th Dec, 2025--- after meeting with Matthias and Ercan.
1. Add Moderate deviation and concentration inequation in Section 3.5 for $U$-statistics and then apply to subgraph counts.
2. Discuss non-integrable case for $\alpha=d$.
3. Compute exactly asymptotic order of variance of triangle count in non-integrable case.

----------------------------------------
$W_s:=[-s^{1/d}/2,s^{1/d}/2]^d\subset\mathbb{R}^d$.
Define $f:\mathbb{R}^d\times\mathbb{R}^d\to[0,1]$ as follows:
$f$ is radial with radial profile $\bar{f}$, and $\bar{f}$ is asymptotically polynomial decay, i.e., $\bar{f}(r)\sim r^{-\alpha}$, with some $\alpha\in(0,d)$.

Find 
$$
\int_{W_s}\int_{W_s^5}f(x_1,x_2)f(x_2,x_3)f(x_3,x_1)f(x_1,x_4)f(x_4,x_5)f(x_5,x_1)\mathrm{d}(x_1,x_2,x_3,x_4,x_5)
$$

--------------------------------------
15 Jan 2026
For tomorrow's meeting:
1. we need to rewrite the abstract and introducation. Introducing RCM with real-world applications and more literature review (references)
2. Do we need also introduce Poisson U-statistics as part of preliminary

---------------------------------------
5 Feb 2026
For the next meeting on 12 Feb:
1. Should we also move the proof of Corollary 3.4 (special case for the Normal approximation theorem) to Section 5.2
2. we use both $(x_1,x_2)\in\eta^2_{s,\ne}$ and $(z_1,z_2)\in\eta^2_{\ne}\cap\Gamma_s^2$. Better to choose only one. 
3. Corollary 3.4 has been changed, which leads to certain necessary changes to some places where it has been applied, for example, Theorem 4.18, Lemma 4.21, 

--------------------------------------
1st March update:
for next meeting on 6th March
1. the \textcolor{cyan}{???} is still unsolved.
2. improve the formlations for subgraph counts and edge-length functionals in Introduction.
and adding reference for these two applications.
3. mentioning $\eta$ is homogeneous Poisson 
5. comments on our applications
6. Switching the order for Section 3 and Section 4.
