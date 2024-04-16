---
Owner: PPeng, Caikun
tags:
  - Level-5
Last edited time: 2024-03-17T14:14
Course Progress: Finish
Notes Progress: In progress
---
# Website

> [!info] Notice  
> Home  
> [https://moodle.telt.unsw.edu.au/course/view.php?id=78484](https://moodle.telt.unsw.edu.au/course/view.php?id=78484)  

# Textbook

> [!info] UNSW Library - Database Access - https%3a%2f%2fsearch.ebscohost.com%2flogin.aspx%3fdirect%3dtrue%26scope%3dsite%26db%3dnlebk%26db%3dnlabk%26AN%3d158159  
>  
> [https://unsw.alma.exlibrisgroup.com/view/action/uresolver.do?operation=resolveService&package_service_id=57461977550001731&institutionId=1731&customerId=1720](https://unsw.alma.exlibrisgroup.com/view/action/uresolver.do?operation=resolveService&package_service_id=57461977550001731&institutionId=1731&customerId=1720)  

https://1drv.ms/b/s!AuXfaR2IFRyogSfS0QyPgA_TeCUx?e=JFq5xn

# Instructor

Professor W. Zhang

Office room 416 EE&T

Tel 9385 - 4033

Email w.zhang@unsw.edu.au

# Assessment Tasks

|   |   |   |   |
|---|---|---|---|
|Assessment Item|Weight|Assessment Item|Weight|
|Final Examination|60%|Research Presentation|10%|
|Research Project|20%|Research Writing|10%|

  

# Lectures

## Lecture 1, Probability Theory

### Probability Theory

### Random Signals

**Random** **$\to$**﻿ **Unpredictable Variations**

### Probability and Random Variables

- **Relative-Frequency Approach**
    
    **The relative frequency**
    
    $0 \leq \frac{n_A}{n} \leq 1$
    
    **The probability**
    
    $P(A)=\lim_{n\to\infty}\frac{n_A}{n}$
    

### Sample Space

Sample Space, **$S$**﻿

All the samples

Events, **$\varepsilon $**﻿

Compnents in $S$﻿

Probability, $P$﻿

The probability of $\varepsilon$﻿

### Random Variables

A function whose domain is a sample space and whose range is a set of real numbers.

There may be more than one random variable associated with the same random experiment.

### Random Process

Definition:

$ ⁍,$

Two basic properties:

$ 0 \leq F_X(x) \leq 1; \\$

![[Untitled 6.png|Untitled 6.png]]

### Probability Density Function

Definition:

$f_X(x)=\frac d {dx} F_X(x)$

Three basic properties:

$f_X(x_1) \leq f_X(x_2),\ \text{if}\ x_1 \leq x_2;\\$

  

### Joint Random Variables

**Joint distribution function**

$F_{X,Y}(x,y)=P[X\leq x,Y\leq y]$﻿

  

**Joint probability density function**

$f_{X,Y}(x,y)=\dfrac{\partial^2 F_{X,Y}(x,y)}{\partial x \partial y}$﻿

  

**Marginal density distribution**

$f_X(x)=\int_{-\infty}^{\infty}{F_{X,Y}(x,y)dy}$﻿

$f_Y(y)=\int_{-\infty}^{\infty}{F_{X,Y}(x,y)dx}$﻿

### Conditional Probability

P[Y|X] denotes the probability of Y given that X has occurred.

$P[Y|X]=\dfrac{P[X,Y]}{P(X)}$﻿

Statistically independent if the outcome of X does not affect the outcome Y. That is

$P[Y|X]=P[Y]$﻿

$P[X|Y]=P[X]$﻿

$P[X,Y]=P[X]P[Y]$﻿

### Expectation

The weighted sum of the possible outcomes.

For discrete,

$\mu_X = E[X]=\sum_{x}{xP[X=x]}$

For continuous,

$\mu_X=E[X]=\int_{-\infty}^{\infty}{xf_X(x)dx}$

### Variance

$\sigma^2_X=Var(x)=E[(X-\mu_X)^2]=E[X^2]-\mu_X^2$

$\sigma^2_X=Var(x)=\int_{-\infty}^{\infty}(x-\mu_X)^2f_X(x)dx$

### Covariance

$Cov(X, Y) = E[(X − \mu_X)(Y − \mu_Y )] = E[XY] − \mu_X\mu_Y$

where

$E[XY]=\int_{-\infty}^{\infty}\int_{-\infty}^{\infty}xyf_{X,Y}(x,y)dxdy$

If X and Y are independent, it has

$E[XY]=E[X]E[Y]$

Then $Cov(X,Y)=0$﻿, that is

independent $\Rightarrow $﻿ covariance = 0

### Transformation of Random Variables

If $Y=g(X)$﻿, then

$F_Y(y)=F_X(g^{-1}(y))$

### Gaussian Distribution

$f_X(x)=\dfrac{1}{\sqrt{2\pi\sigma^2}}e^{-\tfrac{(x-\mu)^2}{2\sigma^2}}$

Q function

$Q(x)=1-F_X(x)=\dfrac 1 {\sqrt{2\pi}}\int_x^\infty{e^{-\tfrac{s^2}2}}ds$

### The Central Limit Theorem

- The $X_k$﻿ with $k = 1, 2, 3, · · · $﻿, $N$﻿ are statistically independent
- The $X_k$﻿ all have the same probability density function
- Both the mean and the variance exist for each $X_k$﻿

Let

$Y=\sum_{k=1}^{N}X_k$

The normalized random variable

$Z=\dfrac{Y-E[Y]}{\sigma_Y}$

approaches a zero-mean Gaussian random variable with unit variance.

## Random Process

### Properties

- Random processes are functions of **time**.
- Random processes are **random** in the sense that it is not possible to predict exactly what waveform will be observed in the future.
- _**Stationary Process**_: If a random process is divided into a number of time intervals, the various sections of the process exhibit essentially the same statistical properties.
    
    $R_X(t, s) = R_X(t − s) $
    
- _**Covariance**_ of the two random variables $X(t_1)$﻿ and $X(t_2)$﻿ is given by
    
    $Cov(X(t_1),X(t_2))=E[X(t_1)X(t_2)]-E[X(t_1)]E[X(t_2)]$
    
- _**Autocorrelation**_ of Random Process
    
    $R_X(t,s)=e[X(t)X^*(s)]$
    

### Wide-sense Stationary Random Process

- The mean of the random process is a constant independent of time
    
    $E[X(t)]=\mu_X$
    
- The autocorrelation of the random process only depends upon the time difference:
    
    $E[X(t)X^*(t-\tau)]=R_X(\tau)$
    

### Properties of Autocorrelation Function

- Power of a Wide-Sense Stationary Process
    
    $R_X(0)=E[X(t)X(t)]=E[|X(t)|^2]$
    
- Symmetry
    
    $R_X(\tau)=E[X(t)X(t-\tau)]=E[X(t-\tau)X(t)]=R_X(-\tau)$
    
- Maximum Value
    
    $R_X(\tau)\leq R_X(0)$
    

![[Untitled 1 4.png|Untitled 1 4.png]]

### Ergodic Process

Ensemble averages of the random process at time $t = t_k$﻿

$E[X(t_k)]=\dfrac 1 N \sum_{j=1}^{N}x_j(t_k)$

The time average of a continuous sample function drawn from a real-valued process is given by

$\varepsilon[x(t)]=\lim_{T\to\infty}{\dfrac 1 {2T} \int_{-T}^T{x(t)dt}}$

A process is said to be ergodic if its **statistical properties** (such as its mean and variance) can **be deduced** from a single, sufficiently long sample (realization) of the process.

_**In other words, those statistics do not change with time.**_

## Lecture 2, Introduction to Inf. Theory

### Entropy, Joint Entropy, Conditional Entropy

- Entropy
    
    $H(X)=-\sum_{x\in X}p(x)\log{p(x)}=\sum_{x\in X}p(x)\log{\frac{1}{p(x)}}$
    
    If $E[\cdot]$﻿ is the expectation, $H(X)=E[\log\tfrac{1}{p(x)}]$﻿
    
- Joint Entropy
    
    $H(X,Y)=-\sum_{x\in X}\sum_{y\in Y}p(x,y)\log p(x,y)$
    
    $H(X,X)=$﻿
    
- Conditional Entropy
    
    $H(Y|X)=-\sum_{x\in X}\sum_{y\in Y}p(x,y)\log p(y|x)$
    
    $H(X|Y)\neq H(Y|X)$﻿
    
    $H(X|X)=0$﻿
    
- Chain Rule
    
    $H(X,Y)=H(X)+H(Y|X)$﻿
    
    $H(X,Y|Z)=H(X|Z)+H(Y|X,Z)$﻿
    

### Relative Entropy, Mutual Information, Venn Diagram

- Relative Entropy or Kullback Leibler distance
    
    $D(p||q)=\sum_{x\in X}p(x)\log \dfrac{p(x)}{q(x)}\geq 0$
    
- Mutual Information
    
    Consider two random variables X and Y with a **joint probability mass function** $p(x, y)$﻿ and **marginal probability mass functions** $p(x)$﻿ and $p(y)$﻿. The mutual information $I(X; Y)$﻿ is defined as
    
    $I(X;Y)=\sum_{x\in X}\sum_{y\in Y}{p(x,y)\log{\dfrac{p(x,y)}{p(x)p(y)}}}\geq0$
    
- Relationship between I and H
    
    $I(X;Y)=H(X)-H(X|Y)$﻿
    
    $I(X;Y)=H(Y)-H(Y|X)$﻿
    
- Venn Diagram of I and H
    
    ![[Untitled 2 4.png|Untitled 2 4.png]]
    

### Chain Rules

- Chain Rule for Entropy
    
    $H(X_1,X_2,...,X_n)=\sum_{i=1}^{n}{H(X_i|X_{i-1},...,X_1)}$
    
    $p(x_1,...,x_n)=\prod_{i=1}^n{p(x_i|x_{i-1},...,x_1)}$
    
- Chain Rule for Information
    
    $I(X_1,X_2,...,X_n;Y)=\sum_{i=1}^{n}I(X_i;Y|X_{i-1},...,X_1)$
    

### Information Inequality

- Let p(x), q(x), x ∈ X, be two probability mass functions. Then
    
    $D(p||q)\geq0$
    
    with equality if and only if
    
    $p(x)=q(x),\ \text{for all }x$
    
- Let $|\mathcal{X}|$﻿ denote the number of elements in the range of $X$﻿. Then
    
    $H(X)\leq\log|\mathcal{X}|$
    
    with equality if and only if $X$﻿ has a uniform distribution over $\mathcal{X}$﻿.
    
- (Independence bound on entropy):  
    Let  
    $X_1, X_2, · · · , X_n$﻿ be drawn according to $p(x_1, x_2, · · · , x_n)$﻿. Then
    
    $H(X_1,X_2,...,X_n)\leq\sum_{i=1}^{n}H(X_i)$
    
    with equality if and only if the $X_i$﻿ are independent.
    

## Lecture 3 Channel Capacity

### Discrete Memoryless Channel

- A Communication System
    
    ![[Untitled 3 3.png|Untitled 3 3.png]]
    
- Discrete Memoryless Channel (DMC)
    - Discrete Channel
        
        a system consisting of an input alphabet $\mathcal{X}$﻿ and output alphabet $\mathcal{Y}$﻿ and a **probability transition matrix** $p(y|x)$﻿ that expresses the probability of **observing** the output symbol $y$﻿ given that we **send** the symbol $x$﻿.
        
    - Memoryless
        
        If the probability distribution of the output depends **only on the input at that time** and is **conditionally independent** of previous channel inputs or outputs.
        
- Binary Symmetric Channel (BSC)
    
    $\mathcal{A}_X=\{0,1\}.\ \mathcal{A}_Y=\{0,1\}.\ P(y=1|x=0)=p(y=0|x=1)=f.$
    
    ![[Untitled 4 3.png|Untitled 4 3.png]]
    
- Binary Erasure Channel (BEC)
    
    $\mathcal{A}_X = \{0, 1\}.\ \mathcal{A}_Y = \{0, ?, 1\}. P(y =?|x = 0) = P(y =?|x = 1) = f . $
    
    ![[Untitled 5 3.png|Untitled 5 3.png]]
    
- Z Channel
    
    $\mathcal{A}_X = \{0, 1\}.\ \mathcal{A}_Y = \{0, 1\}. P(y = 0|x = 1) = f . $
    
    ![[Untitled 6 2.png|Untitled 6 2.png]]
    
- Information Transmission
    - Example 1
        
        Consider **BSC** with $f=0.15$﻿ and $Pr(x=0)=0.9$﻿, $Pr(x=1)=0.1$﻿. Find $I(X;Y)$﻿
        
        - Answer
            
            $I(X;Y)=H(Y)-H(Y|X)\\H(Y)=p(y=0)\log{\tfrac{1}{p(y=0)}}+p(y=1)\log{\tfrac{1}{p(y=1)}}\\H(Y|X)=p(X=0)H(Y|X=0)+p(X=1)H(Y|X=1)$﻿
            
    - Example 2
        
          
        

### Channel Capacity

The capacity of a channel is:

$C=\max_{\mathcal{P}_X}I(X;Y)$

The distribution $\mathcal{P_X}$﻿ that achieves the maximum is called the **optimal input distribution**, denoted by $\mathcal{P}^*_X$﻿.

- Properties of Channel Capacity
    - $C\geq0$﻿, since $I(X;Y)\geq0$﻿
    - $C\geq\log|\mathcal{X}|$﻿ since $C=\max I(X;Y)\leq\max H(X)=\log|\mathcal{X}|$﻿
    - $C\leq\log|\mathcal{Y}|$﻿
    - $I(X;Y)$﻿ is a continuous function of $p(x)$﻿
- BSC Capacity
    
    $C=1-H_2(f)$﻿
    
    $H_2(f)=f\log_2 \dfrac 1 f+(1-f)\log_2\dfrac{1}{1-f}$﻿
    
    The optimal input distribution is $\{0.5, 0.5\}$﻿.
    
    Define $p\triangleq Pr(x=0)$﻿, then $Pr(x=1)=1-p$﻿
    
    $I(X;Y)=H(Y)-H(Y|X)=H_2(a)-H_2(f)$
    
    where $a=p(1-f)+(1-p)f$﻿
    
- BEC Capacity
    
    $C=1-f$﻿
    
    The optimal input distribution is $\{0.5, 0.5\}$﻿.
    
    Define $p\triangleq Pr(x=0)$﻿, then $Pr(x=1)=1-p$﻿
    
    $I(X;Y)=H(X)-H(X|Y)=H_2(p)-fH_2(p)=(1-f)H_2(p)$
    
    The maximum of $I(X:Y)$﻿ is achieved when $P=0.5$﻿
    
- Z Channel Capacity
    
    $C=H_2(p(1-f))-pH_2(f)$﻿
    
    $p=[(1-f)(1+2^{H_2(f)/(1-f)})]^{-1}$﻿
    
    The optimal input distribution is $\{1 − p, p\}$﻿.
    
- Sketch of Capacities
    
    ![[Untitled 7.png]]
    

Channel Coding Theorem

For every DMC, the channel capacity

$C=\max_{\mathcal{p}_X}{I(X;Y)}$

has the following property:

For any $\epsilon > 0$﻿ and $R < C$﻿, there exists a code such that the maximum probability of error is < $\epsilon$﻿.

Conversely, any code sequence with probability of error $→ 0$﻿ must have $R \leq C$﻿

## Lecture 4 Gaussian Channel

### Differential Entropy

$h(X)=-\int_{S}f(x)\log f(x)dx$

$h(X)$﻿ is also written as $h(f)$﻿.

- **Joint Differential Entropy**
    
    $h(X_1,X_2,...,X_n)=-\int f(x_1,x_2,...,x_n)\log f(x_1,x_2,...,x_n)dx_1dx_2\cdots dx_n$﻿
    
    …… more info in L04
    
- Conditional Differential Entropy
    
    $h(X|Y)=-\int{f(x,y)\log{f(x|y)dxdy}}$
    
    $f(x|y)=f(x,y)/f(y)$﻿
    
    $\Rightarrow h(X|Y)=h(X,Y)-h(Y)$﻿
    
- Relative Entropy of Continuous RVs
    
    $D(f||g)=\int{f\log{\dfrac{f}{g}}}$
    
- Mutual Information of Cont. RVs
    
    $I(X;Y)=\int{f(x,y)\log{\dfrac{f(x,y)}{f(x)f(y)}}dxdy}$
    
    $I(X;Y)=h(X)-h(X|Y)=h(Y)-h(Y|X)$﻿
    
    $I(X;Y)=D(f(x,y)||f(x)f(y))$﻿
    
    $I(X;Y)\geq0$﻿ with equality if X and Y are independent
    
- Properties of Differential Entropy
    
    $h(X+c)=h(X)$﻿
    
    $h(aX)=h(X)+\log{|a|}$﻿
    
    $h(X_1,X_2,\cdots,X_n)\leq\sum_{i=1}^{n}{h(X_i)}$﻿
    
    $h(X)\leq\tfrac 1 2\log{((2\pi e)^n |K|)}$﻿ for all $E(XX')=K$﻿
    

### Gaussian Channel

![[Untitled 8.png]]

$Y_i=X_i+Z_i,\ Z_i \sim\mathcal{N}(0,N)$﻿

The information capacity of GC with power constraint P is

$C=\max_{p(x):E(X^2)\leq P}I(X;Y)$

The capacity with power P and noise variance N is

$C=\dfrac 1 2\log{\left(1+\dfrac P N\right)}\text{bits}$

- Band-limited Channel
    
    bandwidth $W$﻿, power constraint $P$﻿, noise spectral density $N_0/2$﻿ watts/Hz
    
    $C=W\log{\left(1+\dfrac{p}{N_0W}\right)}\text{bits per second}$
    

### Parallel Gaussian Channels

![[Untitled 9.png]]

- Water-filling Solution
    
    ![[Untitled 10.png]]
    

## Lecture 5 Coding Techniques

### Repetition Codes

Transmit the message {0 0 1 0}

Encoder Rn: Repeat every bit n times

R3 : {000 000 111 000}

Receive bits {000 100 110 000}

Decoder: Majority-Vote

The probability of error of Rn is

$P_n=\sum_{j=(n+1)/2}^n{\left(\begin{matrix}n\\j\end{matrix}\right)}f^j(1-f)^{n-j}$

### Linear block codes

k bits Data block $\to$﻿ Channel encoder $\to$﻿ n bits codeword

Redundant bits: $n-k$﻿

Code rate: $R_c=\dfrac k n$﻿

- Encoding in (n,k) block code
    
    $U=mG$﻿
    
    $(u_1,u_2,\cdots,u_n)=(m_1,m_2,\cdots,m_n)\cdot\begin{bmatrix}V_1\\V_2\\\vdots\\V_k\end{bmatrix}$﻿
    
    The rows of G, are linearly independent
    
- Systematic block code (n,k)
    
    $G=[P|I_k]$﻿
    
    $I_k=k\times k\text{ identity matrix}$﻿
    
    $P=k\times(n-k) \text{ matrix}$﻿
    
    For any linear code we can find a matrix H
    
    $GH^T=0$
    
    $H=[I_{n-k}|P^T]$
    
    Receive data $r=U+e$﻿
    
    Error pattern or vector: $e$﻿
    
    - Syndrome testing
        
        $S=rH^T=eH^T$﻿
        
- Hamming Codes (n,m)
    
    Code length: $n=2^m-1$﻿
    
    Number of information bits: $k=2^m-m-1$﻿
    
    Number of parity bits: $n-k=m$﻿
    
    Error correction capability: $t=1$﻿
    
    $G=[I_{k\times k}|P]$﻿
    
    - Representation of encoding for Hamming code (7,4)
        
        ![[Untitled 11.png]]
        
- Convolutional codes
    
    Coding rate: $R_c=k/n$﻿
    
    Constraint length $K$﻿
    
    Effective code rate:
    
    L is the number of data bits
    
    $R_{eff}=\dfrac L {n(L+K-1)}<R_c=\dfrac 1 n$
    
    ![[Untitled 12.png]]
    
    Rate 1/2 Convolutional encoder with $g_1=(111),\ g_2=(101)$﻿
    
- State diagram
    
    ![[Untitled 13.png]]
    
- Trellis
    
    ![[Untitled 14.png]]
    
    ![[Untitled 15.png]]
    

## Lecture 6 MIMO Theory

## Review of Gaussian RVs and Entropy

### Entropy

For discrete,

$H(X)=-\sum_{x\in X}p(x)\log{p(x)}=\sum_{x\in X}p(x)\log{\frac{1}{p(x)}}$

For continuous,

$h(X)=-\int_{S}f(x)\log f(x)dx$

### RV and Vector

If x is a real-valued Gaussian Random Variable (RV) with mean $\mu$﻿ and variance $\sigma^2$﻿, its PDF is

$\phi(x)=\dfrac1 {\sqrt{2\pi\sigma^2}}e^{-(x-\mu)^2/(2\sigma^2)}$

We say that $x\sim\mathcal{N}(\mu,\sigma^2)$﻿

If a real-valued vector $\textbf{x}=\begin{bmatrix}x_1&x_2&\cdots&x_n\end{bmatrix}^T$﻿, the joint PDF is

$f(\textbf{x})=\dfrac{\exp{(-\tfrac1 2 (\textbf{x}-\mu_{\textbf{x}})^T\textbf{R}_{\textbf{x}}^{-1}(\textbf{x}-\mu_{\textbf{x}}))}}{(2\pi)^{n/2}\cdot|\textbf{R}_{\textbf{x}}|^{1/2}}$

$\textbf{x}\sim\mathcal{N}(\mu_\textbf{x},\textbf{R}_\textbf{x})$﻿

$|\textbf{R}_{\textbf{x}}|$﻿ denotes the determinant of $\textbf{R}_\textbf{x}$﻿

The vector $\mu_\textbf{x}$﻿ denotes the expected value of the Gaussian random vector $\textbf{x}$﻿ and $\textbf{R}_\textbf{x}$﻿ its covariance matrix

A complex RV $x=y+jz$﻿ is **circularly symmetric** if $y$﻿ and $z$﻿ are independent Gaussian RVs with the same variance $\sigma^2/2$﻿.

We write $x\sim\mathcal{N}_C(\mu,\sigma^2)$﻿, and PDF is

$f(x)=\dfrac1{\pi\sigma^1}\exp(-|x-\mu|^2/\sigma^2)$

Gaussian if

$\textbf{y}\triangleq\begin{bmatrix}\mathcal{R}(\textbf{x})\\\mathcal{J}(\textbf{x})\end{bmatrix}\in\mathbb{R}^{2n}\sim\mathcal{N}(\mu_\textbf{y},\textbf{R}_\textbf{y})$

and

$\textbf{R}_\textbf{y}=\dfrac1 2\begin{bmatrix}\mathcal{R}(\textbf{R}_\textbf{x})&-\mathcal{J}(\textbf{R}_\textbf{x})\\\mathcal{J}(\textbf{R}_\textbf{x})&\mathcal{R}(\textbf{R}_\textbf{x})\end{bmatrix}$

The PDF of $\textbf{x}$﻿ is

$f(\textbf{x})=\pi^{-n}|\textbf{R}_\textbf{x}|^{-1}\exp\left(-(\textbf{x}-\mu_\textbf{x})^H\textbf{R}_\textbf{x}^{-1}(\textbf{x}-\mu_\textbf{x})\right)$

$\textbf{x}\sim\mathcal{N}_C(\mu_\textbf{x},\textbf{R}_\textbf{x})$﻿

### Entropy of Gaussian Random Variable

For $x\sim\mathcal{N}(0,\sigma^2)$﻿

$h(x)=\dfrac1 2\log{(2e\pi\sigma^2)}\text{bits}$

For $\textbf{x}=[x_1\ x_2\ \cdots\ x_n]^T$﻿ is distributed as $\textbf{x}\sim\mathcal{N}(0,Q)$﻿

$\begin{align*}$

### Entropy of Circular Gaussian Vector

For $\textbf{x}=[x_1\ x_2\ \cdots\ x_n]^T$﻿ is distributed as $\textbf{x}\sim\mathcal{N}(0,\Upsilon)$﻿

$\begin{align*}$

### Gaussian vectors maximize capacity

Let **x be a real-valued vector with** **$E[\textbf{x}]=0$**﻿ **and** **$E[\textbf{x}\textbf{x}^T]=\textbf{R}_\textbf{x}$**﻿

Then h(**x**) is maximized if $\textbf{x}\sim\mathcal{N}(0,\textbf{R}_\textbf{x})$﻿

## MIMO Channel Capacity

![[Untitled 16.png]]

$y=\textbf{Hx}+\textbf{n}\\$

where

x are the transmitted complex symbols

y are the received symbols

$\textbf{n}\sim\mathcal{N}_C(0,\sigma^2\textbf{I}_N)$﻿

$h_{i,j} $﻿ denotes the channel gain

## Ergodic Capacity and Outage Capacity

# Lecture 7 Space-Time Coding

## Diversity Techniques

## Alamouti Space-Time Code

## Error Analysis for MIMO Channels

## Other STBC

# OFDM

## OFDM basic

## ISI Channel

## An in-depth study of OFDM

## MIMO-OFDM