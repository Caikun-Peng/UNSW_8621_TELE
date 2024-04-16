---
Owner: PPeng, Caikun
tags:
  - Level-5
Last edited time: 2024-04-09T15:20
Course Progress: In Progress
Notes Progress: Not started
---
# Website

> [!info] Notice | UNSW  
> Staff Help  
> [https://moodle.telt.unsw.edu.au/course/view.php?id=81774](https://moodle.telt.unsw.edu.au/course/view.php?id=81774)  

# Textbook

[https://1drv.ms/b/s!AuXfaR2IFRyojEed89nnTOdmjRl9?e=Sxgnw2](https://1drv.ms/b/s!AuXfaR2IFRyojEed89nnTOdmjRl9?e=Sxgnw2)

[https://1drv.ms/b/s!AuXfaR2IFRyojEggwFTwkJqIqkHv?e=qrDsYb](https://1drv.ms/b/s!AuXfaR2IFRyojEggwFTwkJqIqkHv?e=qrDsYb)

# Instructor

|   |   |   |   |   |
|---|---|---|---|---|
|Convenor|Prof. Jinhong Yuan|j.yuan@unsw.edu.au|EE 408|93854244|
|Lecturer|Dr. Qingqing Cheng|qingqing.cheng@unsw.edu.au|||
|Lecturer|Dr. Min Qiu|min.qiu@unsw.edu.au|||

# Assessment Tasks

|   |   |
|---|---|
|Assessment Item|Weight|
|Homework|15%|
|Mid-Term Examination|35%|
|Final Examination|50%|

# Lectures

![[LECTURE1_2024.pdf]]

![[LECTURE2_2024.pdf]]

![[LECTURE3_2024.pdf]]

![[LECTURE4_2024.pdf]]

![[LECTURE5_2024(1).pdf]]

![[LECTURE5_2024(2).pdf]]

### Lecture 1: Introduction (Not Important)

- Wireless Networking: an Overview (No Need to Review)
    - Challenges in Wireless Communications
        
        Wireless channel is an unpredictable and difficult communications media.
        
        Radio spectrum is a scarce resource, and it can be very expensive. It must be used extremely efficiently.
        
        Security is difficult to implement.
        
        Wireless networking issues, location, mobility, network dynamics  
        (Traffic patterns, user locations, and network conditions are constantly changing.)  
        
        Interfacing between wireless and wired networks with different performance capabilities is a difficult task.
        
        Cross-layer design and optimization is challenging.
        
    - Share resources
        
        Time: TDMA
        
        Frequency: FDMA
        
        Code: CDMA
        
        Source: SDMA
        
          
        

### Lecture 2: Wireless Channel Modeling

- Wireless Channel Brief
    
    Channel varies at two spatial scales:
    
    Large Scale Fading & Small Scale Fading
    
    Wireless channels are fading channels, extremely random and highly unpredictable.
    
    AWGN Channel: $y(t)=ax(t)+n(t)$﻿
    
    Fading Channel: $y(t)=a(t)x(t)+n(t)$﻿
    
- Path Loss and Shadowing
    
    Variations in Fading Channels
    
    ![[Untitled 17.png|Untitled 17.png]]
    
    - Path Loss: Free Space Model
        
        Path loss for unobstructed line of sight (LOS) path
        
        $P_R=P_TG_TG_R\left(\frac{\lambda}{4\pi d}\right)^2$
        
        $P_R$﻿: Receives power
        
        $G_R$﻿: Receiving antenna Gain
        
        $P_T$﻿: Transmitted power
        
        $G_T$﻿: Transmitting antenna Gain
        
        $\overline{PL}(\text{dB})=10\log\frac{P_T}{P_R}=-10\log\left[\frac{G_TG_R\lambda^2}{(4\pi)^2d^2}\right]\\$
        
    - Path Loss: Ray Tracing Models
        
        Ground reflection model (two-ray model)
        
        ![[Untitled 1 5.png|Untitled 1 5.png]]
        
        $P_R=P_TG_RG_T\left(\frac{h_Th_R}{d^2}\right)^2$
        
    - Path Loss: Simplified Path Loss Model
        
        $\begin{array}{rcl}$
        
    - Shadowing: Log-normal distribution
        
        Shadowing typically follows a log-normal distribution given by
        
        $p(\psi_\text{dB})=\dfrac{1}{\sqrt{2\pi}\sigma_{\psi_{\text{dB}}}}\exp\left[-\dfrac{(\psi_\text{dB}-\mu_{\psi_\text{dB}})^2}{2\sigma_{\psi_\text{dB}}^2}\right],\ \psi_\text{dB}=10\log\dfrac{P_T}{P_R}$
        
    - Combined Path Loss and Shadowing
        
        $\overline{PL}(d)+\psi_\text{dB}=PL(d_0)+10n\log\dfrac{d}{d_0}+\psi_text{dB}\\$
        
- Multipath Fading
    - Rayleigh fading
        
        Large collection of reflected waves each about the same without  
        LOS. Appropriate for macrocells in urban environments.  
        
        ![[Untitled 2 5.png|Untitled 2 5.png]]
        
        The probability density function of a Rayleigh distribution is
        
        $P_{R}\left(r\right)=\dfrac{r}{\sigma^{2}}\exp{\left(-\dfrac{r^{2}}{2\sigma^{2}}\right)},\ r\ge0$
        
    - Rician fading
        
        Large collection of reflected waves plus a relatively strong LOS.  
        Appropriate for microcells.  
        
        ![[Untitled 3 4.png|Untitled 3 4.png]]
        
        The probability density function of a Ricean distribution is
        
        $P_R(r)=\dfrac{r}{\sigma^2}\exp{\left(-\dfrac{r^2+s^2}{2\sigma^2}\right)}I_0\left(\dfrac{rs}{\sigma^2}\right),\ r\ge0$
        
        Where $I_0(\cdot)$﻿ is the modified Bessel function of zeroth order, $I_0(x)=\sum_{n=0}^\infty{\frac{\left({x}/{2}\right)^{2n}}{\left(n!\right)^{2}}}$﻿
        
        Rician factor: $K=\dfrac{s^2}{2\sigma^2}$﻿
        
- Physical and Statistical Models
    - Physical Models
        
        Wireless channels can be modeled as linear time-varying systems:
        
        $y(t)=\sum_i{a_i(t)x(t-\tau_i(t))}$﻿, $a_i(t)$﻿ is the gain and $\tau_i(t)$﻿ is the delay
        
        The time-varying impulse response is:
        
        $h(t,\tau)=\sum_i{a_i(t)\delta(\tau-\tau_i(t))}$﻿
        
        When the channel is time-invariant,
        
        $h(\tau)=\sum_i{a_i\delta(\tau-\tau_i)}$﻿
        
    - Passband to Baseband Conversion
        
        Communication takes place at $[f_c-W/2,f_c+W/2]$﻿
        
        Processing takes place at baseband $[-W/2,W/2]$﻿
        
        ![[Untitled 4 4.png|Untitled 4 4.png]]
        
        Channel Response:
        
        $H_b(f)=H(f+f_c)$﻿
        
        $h_b(\tau)=h(t)e^{-j2pi f_c t}=\sum_i{a_i^b \delta(\tau-\tau_i)}$﻿
        
        $a_i^b=a_ie^{-j2pi f_c \tau_i}$﻿
        
        The baseband equivalent channel:
        
        $y_b(t)=\sum_i{a_{i}^{b}x_{b}(t-\tau_{i}(t))}$﻿
        
    - Modulation and Sampling
        
        ![[Untitled 5 4.png|Untitled 5 4.png]]
        
        Multipath Resolution
        
        Sampled baseband-equivalent channel model：
        
        $y[m]=\sum_l{h_l x[m-l]}$﻿
        
        $h_i\approx\sum_l{a_ie^{-j2\pi f_c\tau_i}}$﻿
        
        the sum is over all path fall in the delay bin:
        
        $[\dfrac{l}{W}-\dfrac{1}{2W},\ \dfrac{l}{W}+\dfrac{1}{2W}]$﻿
        
        System resolves the multipaths up to delays of $1/W$﻿
        
    - Flat and Frequency-Selective Fading
        
        $h_l\approx\sum_l{a_i e^{-j2\pi f_c \tau_i}}$﻿
        
        Delay Spread $T_d:=\max_{i,j}{|\tau_i(t)-\tau_j(t)|}$﻿
        
        Coherence Bandwidth $W_c:=1/T_d$﻿
        
        Fading type:
        
        $T_d\ll 1/W,\ W_c\gg W \Rightarrow \textbf{single tap, flat fading}$﻿
        
        $T_d>1/W, W_c<W\Rightarrow\ \textbf{multiple taps, frquency selective fading}$﻿
        
    - Time Variations: General
        
        $y[m]=\sum_l{h_l[m]x[m-l]}$﻿
        
        $h_l[m]\approx\sum_i{a_i(t)e^{-j2pi f_c\tau_i(t)}},\ t=m/W$﻿
        
        $f_c\tau'_i(t)$﻿: Doppler shift of the _i_-th path
        
        Doppler Spread
        
        $D_s:=\max_{i,j}|f_c\tau'_i(t)-f_c\tau'_j(t)|$﻿
        
        $\tau'_i(t)=\dfrac{v}{c}\cos\theta_i$﻿
        
        Coherence time
        
        $T_c:=1/D_s$﻿
        
        ![[Untitled 6 3.png|Untitled 6 3.png]]
        
        ![[Untitled 7 2.png|Untitled 7 2.png]]
        
    - Statistical Models
        
        Design and performance analysis based on statistical ensemble of channels rather than specific physical channel.
        
        $h[m]\sim\mathcal{N}(0,\frac 1 2)+j\mathcal{N}(0,\frac 1 2 )\sim \mathcal{CN}(0,1)$﻿
        
        $\mathcal{CN}$﻿: Complex circular symmetric Gaussian
        
        Squared magnitude is exponentially distributed.
        
        Rician model: 1 line-of-sight plus scattered paths
        
        $h[m]\sim\sqrt{\kappa}e^{j\theta}+\mathcal{CN}(0,1)$﻿
        
    - Additive Gaussian Noise
        
        Complete baseband-equivalent channel model:
        
        $y[m]=\sum_l{h_l[m]x[m-l]+w[m]}$﻿
        
        $w[m]\sim\mathcal{CN}(0,N_0)$﻿
        
        Special case: Flat Fading
        
        $y[m]=h[m]x[m]+w[m]$﻿
        

### Lecture 3: Time Diversity

- Error Probability
    - Constellations
        
        Constellation Energy $\mathcal{E}_s:=E_s\left[|s[n]|^2\right]$﻿
        
        Assume $s[n]$﻿ is an i.i.d. random variable with PDF $P_s[m]$﻿
        
        $\mathcal{E}=E\left[|s[n]|^2\right]=\sum\limits_{m=0}^{M-1}{|s_m|^2P_s[m]}$﻿
        
        If the symbols are equally likely and zero mean
        
        $\mathcal{E}=\dfrac{1}{M}\sum\limits_{m=0}^{M-1}|s_m|^2$﻿
        
        Normalize $\mathcal{C}$﻿ such that $\mathcal{E}_s=1$﻿ to control transmit power
        
        $\mathcal{C}_\alpha=\{\alpha s_0,...\alpha s_{M-1}\},\ \alpha=\sqrt{\dfrac{1}{\dfrac{1}{M}\sum\limits_{m=0}^{M-1}|s_m|^2}}$﻿
        
          
        
    - Baseline: AWGN Channel
        
        Received signal: $y=u+w$﻿
        
        Maximum a posteriori probability (MAP) detection
        
        $u_A$﻿ if $\mathbb{P}\{u=u_A|y\}\ge\mathbb{P}\{u=u_B|y\}$﻿
        
        Maximum likelihood (ML) detection
        
        $u_A$﻿ if $P(y|u_A)>P(y|u_B)$﻿
        
        $\to \dfrac{1}{\sqrt{\pi N_0}}\exp{\left(-\dfrac{(y-u_A)^2}{N_0}\right)}\ge \dfrac{1}{\sqrt{\pi N_0}}\exp{\left(-\dfrac{(y-u_B)^2}{N_0}\right)}$﻿
        
        $\to |y-u_A|<|y-u_B|$﻿
        
        Example
        
        ![[Untitled 8 2.png|Untitled 8 2.png]]
        
        AWGN Channel $\mathcal{X}\sim N_0(u,\sigma^2)$﻿
        
        $u_A$﻿ was transmitted if $y<\frac{u_A+u_B}{2}$﻿, the detector makes an error if $y>\frac{u_A+u_B}{2}$﻿
        
        Error Probability
        
        $\begin{array}{rcl}$
        
          
        
    - Rayleigh Flat Fading Channel
        
        For BPSK
        
        $x=\pm a,\ y=hx+w, h\sim\mathcal{CN}(0,1)$﻿
        
        Coherent detection: we assume that the channel gains are known at the receiver (by sending a pilot or training sequence)
        
        $r:=\Re\{(h/|h|)^*y\}=|h|x+z,\ z\sim N(0,N_0/2)$﻿
        
        Conditional on h (given a realization of h)
        
        $p_e=Q(\sqrt{2|h|^2\text{SNR}})$﻿
        
        at high SNR
        
        $p_e=\dfrac1 2\left(1-\sqrt{\dfrac{\text{SNR}}{1+\text{SNR}}}\right)\approx\dfrac{1}{4\text{SNR}}$﻿
        
- Diversity Techniques
    
    Basic Concept
    
    Same information is sent over independent fading paths
    
    Signals are combined to combat the fading effects.
    
    Design Issues
    
    Methods to obtain diversity branches
    
    Diversity combining methods
    
    Different Classifications
    
    Transmitter vs. receiver
    
    Microscopic vs. macroscopic
    
    Frequency Diversity
    
    Time/Temporal Diversity
    
    Space Diversity
    
- Repetition Coding
    - Simplest Code: Repetition Code
        
        After interleaving over L coherence time periods,
        
        $y_l=h_lx_l+w_l, l=1,...,L$﻿
        
        Repetition coding:
        
        $x_l=x $﻿ for all $l$﻿
        
        $\mathbf{y}=\mathbf{h}x+\mathbf{w}$﻿
        
        where
        
        $\mathbf{y}=[y_1,...,y_L]^t,\ \mathbf{h}=[h_1,...,h_L]^t,\ \mathbf{w}=[w_1,...,w_L]^t$﻿
        
    - Geometry
        
        For BPSK $x=\pm a$﻿
        
        $\mathbf{u}_A=+a\mathbf{h},\ \mathbf{u}_B=-a\mathbf{h}$﻿
        
        $\Rightarrow\~y=\dfrac{\mathbf{h}^*}{\|\mathbf{h}\|}\mathbf{y}=\dfrac{\mathbf{h}^*}{\|\mathbf{h}\|}(\mathbf{h}x+\mathbf{w})=\|\mathbf{h}\|x+\dfrac{\mathbf{h}^*}{\|\mathbf{h}\|}\mathbf{w}=\|\mathbf{h}\|x+w'$﻿
        
        The conditional error probability
        
        $p_e(e|\mathbf{h})=Q(\sqrt{2\|\mathbf{h}\|^2\text{SNR}})$﻿
        
        $f(\|\mathbf{h}\|^2)=f(x)=\dfrac{1}{(L-1)!}x^{L-1}e^{-x},\ x\ge0$﻿
        
        ![[Untitled 9 2.png|Untitled 9 2.png]]
        
        The average error probability
        
        $\begin{array}{rcl}$
        
        At high SNR
        
        $\dfrac{1+\mu}{2}\approx1\text{ and }\dfrac{1-\mu}{2}\approx\dfrac{1}{4\text{SNR}}$
        
        $p_e(e)\approx\left(\begin{array}{c}2L-1\\L\end{array}\right)\dfrac{1}{(4\text{SNR})^L}$
        
- Rotation Coding
    - The Transmission System
        
        complex fading channel model: $r’= α’x+n’$﻿, e.g., $x=x1+x2j$﻿
        
        After coherent detection: $r=|α’|x+n = αx+n$﻿, $α$﻿ is real
        
        ![[Untitled 10 2.png|Untitled 10 2.png]]
        
    - Example: Rotation code (L=2)
        
        Transmit two symbols $u_1$﻿ and $u_2$﻿ over two time slots.
        
        The transmitted symbols are encoded by using a rotation matrix
        
        $\mathbf{x}=\mathbf{R}\left[\begin{matrix}u_1\\u_2\end{matrix}\right],\ \mathbf{R}:=\left[\begin{matrix}\cos\theta&-\sin\theta\\\sin\theta&\cos\theta\end{matrix}\right]$﻿
        
        $x_1$﻿, $x_2$﻿ are two BPSK symbols before rotation
        
        $\begin{array}{ll}$
        
        The error probability
        
        $⁍$
        
        ![[Untitled 11 2.png|Untitled 11 2.png]]
        
        Let $\mathbf{u}_A = \begin{bmatrix}$﻿ and $\mathbf{u}_B = \begin{bmatrix}$﻿
        
        $\mathbb{P}\{\mathbf{x}_A \rightarrow \mathbf{x}_B|h_1, h_2\} = Q\left(\dfrac{\lVert \mathbf{u}_A - \mathbf{u}_B \rVert}{\sqrt{2 N_0/2}}\right) = Q\left( \sqrt{\text{SNR}/2 \cdot (\lvert h_1 \rvert^2 d_1^2 + \lvert h_2 \rvert^2 d_2^2)} \right)$﻿
        
        Normalized codeword distance
        
        $\mathbf{d}:=\dfrac 1 a(\mathbf{x}_A-\mathbf{x}_B)=\begin{bmatrix}2\cos\theta\\2\sin\theta\end{bmatrix}$﻿
        
        - Upper bound on the error probability
            
            $\begin{array}{rcl}$
            
            If $d_1\ne0$﻿ and $d_2\ne0 $﻿, at high SNR:
            
            $\mathbb{P}\{\mathbf{x}_A \rightarrow \mathbf{x}_B\}\le\dfrac{16}{|d_1d_2|^2}\text{SNR}^{-2}$﻿
            
        - Product Distance
            
            let $\delta_{AB}=|d_1d_2|^2$﻿
            
            Overall error probability upper bound
            
            $p_e\le16\left(\dfrac{1}{\delta_{AB}}+\dfrac{1}{\delta_{AC}}+\dfrac{1}{\delta_{AD}}\right)\text{SNR}^{-2}\le\dfrac{48}{\min_{j=B,C,D}\delta_{Aj}}\text{SNR}^{-2}$﻿
            
            Find the rotation angle to minimise the worst-case error probability
            
            $\delta_{AB}=\delta_{AD}=4\sin^22\theta$﻿ and $\delta_{AC}=16\cos^22\theta$﻿
            
            $\Rightarrow\theta^*=\dfrac 1 2 \tan^{-1}2$﻿
            
            Product distance = $|d_1||d_2|$﻿.
            
            $|d_1d_2|>0\to$﻿ attain a diversity gain of **2**
            
            Maximise $|d_1d_2|\to$﻿ maximise the coding gain
            

### Lecture 4: Receive and Transmit Diversity

- Receiver Diversity Combining Techniques
    
    ![[Untitled 12 2.png|Untitled 12 2.png]]
    
    - Linear Diversity Combining
        
        Outage probability relative to $\gamma_0$﻿
        
        $P_{out}(\gamma_0)=\Pr(\gamma<\gamma_0)=\int_0^{\gamma_0}\underset{\text{PDF}}{\underline{p_\gamma(\gamma)}}d\gamma=\underset{\text{CDF}}{\underline{P_\gamma(\gamma_0)}}$﻿
        
        In **Rayleigh fading** the outage probability becomes
        
        $P_{out}=\int_0^{\gamma_0}\dfrac{1}{\bar{\gamma}}\exp{(-\gamma/\bar{\gamma})}d\gamma=1-\exp{(-\gamma_0/\bar{\gamma})}$﻿
        
        Array gain
        
        $A_g=\dfrac{\bar{\gamma}_{\Sigma}}{\bar{\gamma}}$﻿
        
        Selection and Threshold combining
        
        all $\alpha_i=0$﻿ except one
        
        Maximal ratio combining
        
        $\alpha_i=r_ie^{-j\theta_i}$﻿
        
        Equal gain combining
        
        $\alpha_i=e^{-j\theta_i}$﻿
        
    - Selection Combining vs Threshold Combing
        - Selection Combining (SC)
            
            Combiner outputs the signal with highest SNR $r_i^2/N_i$﻿
            
            Assuming independent branches, the CDF of $\gamma_{\sum}$﻿ is given by
            
            $\begin{array}{rcl}$
            
            For i.i.d. Rayleigh fading
            
            $\begin{array}{rcl}$
            
            Outage Probability
            
            $p_{out}(\gamma_0)=\Pr(\gamma_{\Sigma}<\gamma_0)=\left(1-\exp(-\gamma_0/\bar{\gamma})\right)^M$﻿
            
            Average SNR of the combiner output
            
            $\bar{\gamma}_{\Sigma}=\int_0^\infty\gamma p_{\gamma_{\Sigma}}(\gamma)d\gamma=\bar{\gamma}\sum\limits_{i=1}^{M}\dfrac 1 i$﻿
            
            Array gain
            
            $A_g=\sum\limits_{i=1}^M\dfrac 1 i$﻿
            
            ![[Untitled 13 2.png|Untitled 13 2.png]]
            
        - Threshold Combining (TC)
            
            _M_ branches are scanned in a fixed sequence. **The first one** above a given  
            threshold is used. The signal is used until it falls below the threshold.  
            
            ![[Untitled 14 2.png|Untitled 14 2.png]]
            
            ![[Untitled 15 2.png|Untitled 15 2.png]]
            
    - Maximal Ratio Combining vs Equal Gain Combing
        - Maximal Ratio Combining
            
            In the general model, set $\alpha=a_ie^{-j\theta_i}$﻿
            
            $r=\sum\limits_{i=1}^{M}\alpha_ir_ie^{j\theta_i}=\sum\limits_{i=1}^{M}a_ie^{-j\theta_i}r_ie^{j\theta_i}=\sum\limits_{i=1}^{M}a_ir_i$﻿
            
            Assuming the same noise power at all the branches
            
            $\gamma_{\Sigma}=\dfrac{r^2}{N_{total}}=\dfrac{1}{N_0}\dfrac{\left(\sum\limits_{i=1}^{M}a_ir_i\right)^2}{\sum\limits_{i=1}^{M}a_i^2}$﻿
            
            In order to maximize $\gamma_{\Sigma}$﻿, based on Cauchy-Schwartz inequality,
            
            $a_i^2=r_i^2/N_0$﻿ and $\gamma_{\Sigma}=\sum\limits_{i=1}^{M}r_i^2/N_0=\sum\limits_{i=1}^{M}\gamma_i$﻿
            
            Average SNR of the combiner output
            
            $\bar{\gamma}_{\Sigma}=\sum\limits_{i=1}^{M}\bar{\gamma_i}=M\bar{\gamma}$﻿
            
            Array gain
            
            $A_g=M$﻿
            
            $\gamma_{\Sigma}$﻿ follows a Chi-squared ($\mathcal{X}^2$﻿) distribution with 2M degrees of freedom,
            
- Sum
    
    ![[Untitled 16 2.png|Untitled 16 2.png]]