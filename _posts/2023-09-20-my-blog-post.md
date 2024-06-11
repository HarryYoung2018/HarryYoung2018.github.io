# Vector Basics

## **Vector**

* $\vec{a}=<a_1,a_2,\ldots,a_n>=\lVert \vec{a} \rVert\cdot\hat{i}$ is a **vector** in $\R^n$
* $\vec{a}$ has **length** $\lVert \vec{a}\rVert=\sqrt{a_1^2+a_2^2+\ldots+a_n^2}$
* $\vec{a}$ points in direction of **unit vector** $\hat{i}=\frac{\vec{a}}{\lVert \vec{a}\rVert}$, where $\lVert\hat{i}\rVert=1$

### Vector triangle inequality $\lVert \vec{a}+\vec{b} \rVert \leq \lVert \vec{a} \rVert+\lVert \vec{b} \rVert$

1. Geometric view

   <img src="https://upload.wikimedia.org/wikipedia/commons/0/08/Vector_triangle_inequality_vw.PNG" alt="File:Vector triangle inequality vw.PNG - Wikimedia Commons" style="zoom:33%;" />

2. Algebraic view
   $$
   \begin{align}
   \lVert \vec{a}+\vec{b} \rVert^2 =&\vec{a}^2+2\left(\vec{a} \cdot \vec{b}\right)+\vec{b}^2\\
   \leq&\lVert\vec{a}\rVert^2+2\left(\lVert \vec{a} \rVert\cdot\lVert\vec{b} \rVert\right)+\lVert\vec{b}\rVert^2=\left( \lVert\vec{a}\rVert+\lVert\vec{b}\rVert \right)^2\\
   \Rightarrow&\lVert\vec{a}+\vec{b}\rVert \leq \lVert\vec{a}\rVert+\lVert\vec{b}\rVert
   \end{align}
   $$
   

---

## Vector dot product

* $\vec{a}\cdot \vec{b}=\sum a_i\cdot b_i=\lVert \vec{a}\rVert \lVert \vec{b}\rVert \cdot \cos{\theta}=scalar$ is **dot product** of **2 vectors** in $\R^n$, $\cos{\theta}=\frac{\vec{u}\cdot \hat{i}}{\lVert\vec{u}\rVert \lVert \hat{i}\rVert}$ is **direction angle** of **2 vectors**, $\mathbf{\vec{a}\cdot \vec{a}=\lVert \vec{a} \rVert^2=\vec{a}^2}$
* $\vec{a}\cdot\vec{b}=\vec{b}\cdot\vec{a}$, $(c\vec{a})\cdot\vec{b}=c(\vec{a}\cdot\vec{b})$, $\vec{a}\cdot\left(\vec{b}+\vec{c}\right)=\vec{a}\cdot\vec{b}+\vec{a}\cdot\vec{c}$
* **orthogonal vectors** have $\theta=\frac{\pi}{2},\cos{\theta}=0\Rightarrow \vec{a}\cdot \vec{b}=0$
* **parallel vectors** have $\theta=0,\cos{\theta}=1\Rightarrow \vec{a}\cdot \vec{b}=\lVert \vec{a}\rVert \lVert \vec{b}\rVert$

### Proof of *Cauchy-Schwarz inequality*

* $\left(ac+bd\right)^2\leq \left(a^2+b^2\right)\left(c^2+d^2\right)$

$$
\begin{align}
\forall \vec{A}=<a,b>&\text{, }\vec{B}=<c,d>\text{ in }\R^2\text{,}\\
\vec{A}\cdot \vec{B}=ac+bd=\lVert \vec{A}\rVert \lVert \vec{B}\rVert \cdot \cos{\theta}&=\sqrt{\left(a^2+b^2\right)\left(c^2+d^2\right)}\cdot \cos{\theta}\\
\left(ac+bd\right)^2=&\left(a^2+b^2\right)\left(c^2+d^2\right)\cdot \cos^2{\theta}\\
\because \cos{\theta}\in[-1,1]\Rightarrow&\cos^2{\theta}\in[0,1]\\
\therefore \left(ac+bd\right)^2\leq &\left(a^2+b^2\right)\left(c^2+d^2\right)\\
\end{align}
$$

* Extended *Cauchy-Schwarz inequality*

$$
\begin{align}
\forall \vec{A}=<a_1,\ldots,a_n>&\text{, }\vec{B}=<b_1,\ldots,b_n>\text{ in }\R^n\text{,}\\
\vec{A}\cdot \vec{B}=\sum_{i=1}^na_i\cdot b_i&=\sqrt{\sum_{i=1}^na_i^2 \cdot\sum_{i=1}^n b_i^2}\cdot \cos{\theta}\\
\left(\sum_{i=1}^na_i\cdot b_i\right)^2&=\sum_{i=1}^na_i^2 \cdot\sum_{i=1}^n b_i^2\cdot \cos^2{\theta}\\
\because \cos{\theta}\in[-1,1]\Rightarrow&\cos^2{\theta}\in[0,1]\\
\therefore \left(\sum_{i=1}^na_i\cdot b_i\right)^2&\leq \sum_{i=1}^na_i^2 \cdot\sum_{i=1}^n b_i^2\\
\end{align}
$$

### Vector projections

* **scalar projection of $\vec{b}$ to $\vec{a}$** is $\mathrm{comp}_a b=l=\lVert \vec{b} \rVert\cdot \cos{\theta}=\frac{\vec{a}\cdot \vec{b}}{\lVert \vec{a} \rVert}$

  > orthogonal decomposition of $\vec{b}$ on direction of $\vec{a}$

* **vector projection of $\vec{b}$ to $\vec{a}$** is $\mathrm{proj}_a b=l\cdot\hat{i}=\left( \frac{\vec{a}\cdot\vec{b}}{\lVert\vec{a}\rVert} \right)\cdot \frac{\vec{a}}{\lVert \vec{a} \rVert}=\mathrm{comp}_a b\, \cdot \frac{\vec{a}}{\lVert \vec{a} \rVert}$

  > vector at direction of $\vec{a}$ with length $\mathrm{comp}_a b$

  <img src="https://calconcalculator.com/wp-content/uploads/2022/01/images-2-1.png" alt="Vector Projection Calculator - Solution with Steps | 2D, 3D" style="zoom:90%;" />

---

## Vector cross product

* $\vec{a}\times\vec{b}=\left| \begin{matrix}\hat{i} & \hat{j} & \hat{k}\\ a_1 & a_2 & a_3\\ b_1 & b_2 & b_3\\ \end{matrix} \right|=\vec{c}=-\vec{b}\times\vec{a}$ is **cross product** of **2 vectors** in $\R^3$ or $\R^7$, $\vec{c}$ is perpendicular to the plane of $\vec{a}$ and $\vec{b}$ and **follows right-hand rule**, **length** of vector $\lVert \vec{c}\rVert=\lVert\vec{a}\times\vec{b}\rVert=\lVert\vec{a}\rVert\lVert\vec{b}\rVert\cdot\sin{\theta}$, $\mathbf{\vec{a}\times\vec{a}=0}$
* **parallel vectors** have $\theta=0,\sin{\theta}=0\Rightarrow\vec{a}\times\vec{b}=0$
* $\vec{a}\cdot(\vec{b}\times\vec{c})=\left| \begin{matrix} a_1 & a_2 & a_3\\ b_1 & b_2 & b_3\\ c_1 & c_2 & c_3\\ \end{matrix} \right|=(\vec{a}\cdot\vec{c})\cdot\vec{b}-(\vec{a}\cdot\vec{b})\cdot\vec{c}$ is **triple product** of **3 vectors** in $\R^3$ or $\R^7$

### Areas of triangle and parallelogram

$S_{\mathrm{para}}=2S_\triangle=l\cdot \lVert b\rVert=\lVert\vec{a}\rVert\lVert\vec{b}\rVert\cdot\sin{\theta}=\lVert\vec{a}\times\vec{b}\rVert$

<img src="C:\Users\yangy\AppData\Roaming\Typora\typora-user-images\image-20240124122921431.png" alt="image-20240124122921431" style="zoom:35%;" />

### Volume of parallelepiped

$V=h\cdot A=\lVert \vec{a}\cdot(\vec{b}\times\vec{c})\rVert$

<img src="C:\Users\yangy\AppData\Roaming\Typora\typora-user-images\image-20231106184805575.png" alt="image-20231106184805575" style="zoom:67%;" />


***

***
