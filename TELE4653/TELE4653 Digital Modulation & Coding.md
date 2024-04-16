---
Owner: PPeng, Caikun
tags:
  - Level-4
Last edited time: 2024-02-21T18:49
Course Progress: In Progress
Notes Progress: In progress
---
# Website

> [!info] Notice | UNSW  
> Staff Help  
> [https://moodle.telt.unsw.edu.au/course/view.php?id=81752](https://moodle.telt.unsw.edu.au/course/view.php?id=81752)  

# Textbook

https://1drv.ms/b/s!AuXfaR2IFRyojDCVHnYDEpdzsJg9?e=NmwVdA

  

# Instructor

Professor W. Zhang

Office room 416 EE&T

Tel 9385 - 4033

Email w.zhang@unsw.edu.au

# Assessment Tasks

|   |   |
|---|---|
|Assessment Item|Weight|
|Final Exam|60%|
|Laboratory Work|20%|
|Assignment 1|10%|
|Assignment 2|10%|

# Lectures

![[Untitled.pdf]]

![[Untitled 1.pdf]]

### L1 Fundamentals

- Introduction to communications
    
    ![[Untitled 2.png|Untitled 2.png]]
    
    - Modulation
        
        Information signal: low frequency signal
        
        Spectrum of the channel: high frequency
        
        **Modulation process: translate the information signal to a higher frequency signal to matches the channel spectrum**
        
        Properties of FT:
        
        ![[Untitled 1 2.png|Untitled 1 2.png]]
        
        ![[Untitled 2 2.png|Untitled 2 2.png]]
        
- Lowpass (LP) and Bandpass (BP) Signals
    
    The Fourier transform of a **real** signal x(t) has _Hermitian symmetry_
    
    $X(-f)=X^*(f) \ \to\ |X(-f)|=|X(f)|\ \&\ \angle X^*(f)=-\angle X(f)$﻿
    
    - Lowpass Signals
        
        ![[Untitled 3.png]]
        
        Usually lowpass signals are low frequency signals
        
        $X_+(f)=\left\{\begin{array}{lr}$
        
        $X_+(f)=X(f)u_{-1}(f), $﻿ $X_-(f)=X(f)u_{-1}(-f).$﻿
        
        The bandwidth of a real lowpass signal is the minimum positive $W $﻿such that $X( f ) = 0$﻿ outside $[−W, +W]$﻿ (_frequency support_)
        
        In general and for all signals, real or complex, the bandwidth is defined as one-half of the frequency support.
        
        $\begin{align*}$
        
        In modulation process, the spectrum of the lowpass message signal is translated to higher frequencies.
        
        The resulting modulated signal is a bandpass signal.
        
    - Bandpass Signals
        
        ![[Untitled 4.png]]
        
        Bandpass signal is a real signal $x(t)$﻿ for which there exists positive $f_0$﻿ and $W $﻿such that the positive spectrum of $X( f )$﻿, i.e.,
        
        $X_+( f )$﻿, is nonzero only in the interval $[ f_0 − W/2, f_0 +W/2]$﻿
        
        $X_-( f )$﻿, is nonzero only in the interval $[ -f_0 − W/2, -f_0 +W/2]$﻿
        
        $X(f)=X_+(f)+X_−(f)=X_+(f)+X^∗_+(f)\to x(t)=x_+(t)+x_-(t)$﻿
        
        $f_0$﻿: central frequency. Bandwidth is $W$﻿
        
    - Lowpass Equivalent of Bandpass Signals
        
        $\begin{align*}$
        
        We define $x_l(t)$﻿, the lowpass equivalent of bandpass signal $x(t)$﻿
        
        And the spectrum of $x_l(t)$﻿ is $X_l(f)=2X_+(f+f_0)=2X(f+f_0)u_{-1}(f+f_0)$﻿
        
        $\begin{align*}$
        
        For simplicity, $x_l(t)=x_i(t)+jx_q(t)$﻿, $i$﻿ means in-phase, $q$﻿ means quadrature
        
        $⁍$
        
        We can get
        
        $x(t)=x_i(t)\cos(2\pi f_0t)+x_q(t) \sin (2 \pi f_0 t )\\$
        
        Also, we can write a similar relation in polar coordinates expressing x(t) in terms of its magnitude $r_x(t)$﻿ and phase $\theta_x(t)$﻿
        
        $\begin{align*}$
        
- Signal Space Concepts
    - Vector Space Concepts
        
        $\begin{array}{ll}$
        
    - Signal Space Concepts
        
        $\begin{array}{ll}$
        
- Expansion of BP Signals
    - Orthogonal Expansion of Signals
        
        - Gram-Schmidt procedure
            
            $\mathbf{v}\in\mathbf{V}^n$﻿, $\mathbf{V}^k$﻿ is the subspace of $\mathbf{V}^n $﻿ with orthogonal set $\{n_1,n_2,...,n_k\}$﻿ and $\mathbf{v}\notin \mathbf{V}^k$﻿
            
            $\begin{array}{rclc}$
            
        
        Using a set of signal $s_m(t),m=1,2,...,M$﻿ to construct a set of orthonrmal waveforms $\phi_n(t)$﻿
        
        1. $\phi_1=\dfrac{s_1(t)}{\sqrt{\mathcal E_1}}$﻿
        2. $\phi_k(t)=\dfrac{\gamma_k(t)}{\sqrt{\mathcal E_K}}\text{ for }k=2,...,N,(N\le M)$﻿
            
            where
            
            $\begin{array}{rcl}$
            
        
        Once constructed $\phi_n(t)$﻿,
        
        $s_m(t)=\displaystyle\sum^N_{n=1}s_{mn}\phi_n(t),\ m=1,2,...,M$
        
    - BP and LP Orthonormal Basis
        
        $\begin{array}{}$
        
        Define
        
        $\begin{align*}$
        
        Then
        
        $s_m(t) = \sum_{n=1}^{N} \left[ \frac{s^{(r)}_{mln}}{\sqrt{2}} \phi_n(t) + \frac{s^{(i)}_{mln}}{\sqrt{2}} \tilde{\phi}_n(t) \right]$
        
        Where we have assumed that $s_{mln}=s_{mln}^{(r)}+js_{mln}^{(i)}$﻿
        

### L2 Digital Modulation

  

### L3

### L4

  

# Tutorial