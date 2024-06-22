---
layout: post
title:  "Binomial Theorem's Insight in a Combinatorics Problem"
date:   2024-06-20 20:17:09 +0800
categories: Mathematics
---

# Interesting Insight in an Olympiad Level Combinatorics Problem

Suppose we were asked to calculate the sum $$S=\frac{1}{2022}\left(\begin{matrix} 1 \\ 2022 \end{matrix}\right)^2+\frac{2}{2021}\left(\begin{matrix} 2 \\ 2022 \end{matrix}\right)+\dots+\frac{2022}{1}\left(\begin{matrix} 2022 \\ 2022 \end{matrix}\right)^2$$

Finding the sum of the combination using the binomial theorem:

$$
\begin{align}
	S&=\frac{1}{2022}\left(\begin{matrix} 1 \\ 2022 \end{matrix}\right)^2+\frac{2}{2021}\left(\begin{matrix} 2 \\ 2022 \end{matrix}\right)+\dots+\frac{2022}{1}\left(\begin{matrix} 2022 \\ 2022 \end{matrix}\right)^2\\
	&=\sum_{i=1}^{k} \frac{i}{k-i+1}\left(\begin{matrix} i \\ k \end{matrix} \right)^2\\
	&=\sum_{i=1}^{k} \frac{i}{k-i+1}\left(\frac{k!}{(k-i)!\cdot i!} \right)^2\\
	&=\sum_{i=1}^{k} \frac{k!}{(k-(i-1))!\cdot (i-1)!}\cdot \left(\begin{matrix} i \\ k \end{matrix} \right)\\
	&=\sum_{i=1}^{k} \left(\begin{matrix} i-1 \\ k \end{matrix} \right)\cdot \left(\begin{matrix} i \\ k \end{matrix} \right)\\
	&=\sum_{i=1}^{k} \left(\begin{matrix} i-1 \\ k \end{matrix} \right)\cdot \left(\begin{matrix} k-i \\ k \end{matrix} \right)\\
\end{align}
$$

This naturally reminds us of the binomial theorem:

> $$
> (x+y)^n=\sum_{k=0}^{n}\left(\begin{matrix} n \\ k \end{matrix} \right)x^ky^{n-k}
> $$

However, an insight into how the two equations relate is needed:

$$
\begin{align}
	(1+x)^k\cdot(1+x)^k&=\left( \left(\begin{matrix} 0 \\ k \end{matrix} \right)+\left(\begin{matrix} 1 \\ k \end{matrix} \right)x+\ldots+\left(\begin{matrix} k \\ k \end{matrix} \right)x^k \right)^2\\
	&=\left(\begin{matrix} m \\ k \end{matrix} \right)x^m\cdot\left(\begin{matrix} n \\ k \end{matrix} \right)x^n\\
	&=\left(\begin{matrix} m \\ k \end{matrix} \right)\left(\begin{matrix} n \\ k \end{matrix} \right)\cdot x^{m+n}\\
\end{align}
$$

Thus, we have our solution:

$$
\begin{align}
	x=0\Rightarrow 1&=\left(\begin{matrix} m \\ k \end{matrix} \right)\left(\begin{matrix} n \\ k \end{matrix} \right)\cdot 0^{m+n}\\
	1 &=\left(\begin{matrix} i-1 \\ k \end{matrix} \right)\left(\begin{matrix} k-i \\ k \end{matrix} \right)\cdot 0^{k-1}\\
	\therefore S&=\sum_{i=1}^{k} \left(\begin{matrix} i-1 \\ k \end{matrix} \right)\cdot \left(\begin{matrix} k-i \\ k \end{matrix} \right)\\
	&=\sum_{i=1}^{k} 1=k\\
\end{align}
$$
