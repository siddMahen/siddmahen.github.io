---
layout: post
title:  "Something Beautiful"
date:   2014-04-12 23:31:00
tags:
  - graph theory
  - triangle free graphs
---

I think it's best to begin with something beautiful.

<div class="prp">
<span class="ref">Mantel, 1907</span> Every triangle free graph on $n$ nodes
has at most $n^2/4$ edges.

<div class="proof">
Let $G$ be a triangle free graph and let $x$ and $y$ be endpoints of an edge
$xy$ in $G$. Because $G$ is triangle free, $x$ and $y$ cannot be
simoultanously adjacent to any other node in $G$. Thus, the sum of their
degrees is at most $n$,

$$ d(x) + d(y) \leq n.$$

If we sum the inequality above for every edge $xy$ in $G$, the degree of each
node $x$ is present exactly $d(x)$ times. Thus, we obtain

$$ \sum_{x \in V(G)}{ d(x)^2 } \leq ne(G).$$

Now, by the Handshaking Lemma, we know that

$$ (2e(G))^2 = \bigg( \sum_{x \in V(G)}{ d(x) } \bigg)^2.$$

Applying Cauchy's inequality along with our results above yields

$$\begin{align*}
    (2e(G))^2 &= \bigg( \sum_{x \in V(G)}{ d(x) } \bigg)^2 \\
             &\leq n\sum_{x \in V(G)}{ d(x)^2 } \\
             &\leq n^2e(G).
\end{align*}$$

It follows that $e(G) \leq n^2/4$.
</div>
</div>

These results also imply that every graph on $n$ nodes with more than $n^2/4$
edges must contain a triangle.

I hope you enjoyed this neat little argument as much as I did, and I look
forward to writing more often.
