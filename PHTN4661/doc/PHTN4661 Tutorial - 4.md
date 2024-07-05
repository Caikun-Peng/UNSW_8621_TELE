---
Owner: Peng, Caikun
Electives: Level 4
Last edited time: 2024-05-03
Course Progress: In Progress
Note Progress: In Progress
Note ID: PHTN4661-Tut-3
---

- Tutorial 4 Waveguide coupling and connection

1. Prove and explain that $\sin\theta_A=\sqrt{n_1^2 - n_2^2} = NA$

    > $n_1 \sin(90\degree-\theta_1) = n_2 \sin\theta_2 = n_1 \cos\theta_1$  
    > $n_0 \sin\theta_A = n_1 \sin\theta_1$
    > $\theta_2 = 90\degree \to \sin\theta_2 = 1$  
    > $n_1\cos\theta_1=n2$  
    > $n_0 = 1 \to \sin\theta_A = n_1\cos\theta_1 =\sqrt{n_1^2(1-cos^2\theta_1)}=\sqrt{n_1^2 - n_1^2\cos^2\theta_1} = \sqrt{n_1^2 - n_2^2}$  

2. #不会 Assuming perfect alignment in the case of launching light from a LED source with its radiation pattern $I = I_0 cos^\sigma{\theta}$, into an SI-MM (step-index multimode) optical fibre, where the air gap between the source and the fibre is kept minimum, the light emitting area of the source is $A_s$ and the area of fibre (core) is $A_f$.  
    Show and explain that the launching efficiency will be
    $$
        \eta = \frac{1}{2} (NA)^2 (\sigma+1) \left\{\begin{aligned}&\frac{A_f}{A_s}&&A_f<A_s\\&1&&A_f>A_s\end{aligned}\right.
    $$
    $$
      d\Omega=\int_{0}^{2\pi}\sin\theta d\phi
    $$
    $$
      P=\int_{0}^{\theta_{\max}}I_0\cos\theta d\Omega
    $$

3. #不会 For the same case as above question, assume that the SI-MM optical fibre has its coating removed and exposed to air with no=1. In this case, when coupling light into fibre core, some power will be coupled into cladding and propagate as cladding modes along the fibre.   
    Considering $A_f > A_s$, work out what fraction of optical power will be launched into cladding and guided along the fibre as cladding modes.   
    Discuss how the cladding modes can affect optical fibre measurements and what measures could be used to avoid or remove the cladding modes.



4. The guided modes, $E_i(x,y) i=1,2, … N$, of an optical waveguide can be excited when a particular optical field $𝑬_𝟎(x,y)$, is launched at the input end of the waveguide, can be determined 
    $$E_0(x,y)=\sum_{i=1}^{N}A_iE_i(x,y)+\text{unguided modes}$$
    1. What is assumed in obtaining the expression above 
        > (Lecture 4, page 11) $E_0$ is decomposed into a linear combination of the guided modal fields and unguided modal fields.  
    1. Explain what $A_i$ means in terms of optical coupling / launching.
        > $A_i$ represents the amplitude coefficient for $i$-th guided mode 
    1. How can $A_i$ be determined? 
        > $$A_i=\frac{\int\int E_0(x,y)E_i^*(x,y)dxdy}{\int\int|E_i(x,y)|^2dxdy}$$
    2. What is the condition to excite one mode only?
        > The wavelength should be within the single-mode range.


5. Assume perfect alignment in the case of launching light from a LD source with its field pattern, expressed as $𝐸_S(𝑟) = 𝑒^{−𝑟^2/2𝜔_𝑠^2}$, at the input end of an SI-SM (step-index single-mode) optical fibre. The fundamental mode field of the fibre under Gaussian approximation can be expressed as $𝐸_f(𝑟) = 𝑒^{−𝑟^2/2𝜔_𝑓^2}$.   
    Derive the launching efficiency for this case in a step-by step approach.

    > $$\begin{align*}\eta 
      &= \frac{\left|\displaystyle\int_{0}^{\infty}{E_S(r)E_f(r)dr}\right|^2}{\displaystyle\int_{0}^{\infty}{\left|E_S(r)\right|^2dr}\displaystyle\int_{0}^{\infty}{\left|E_f(r)\right|^2dr}} \\
      &= \frac{\left|\displaystyle\int_{0}^{\infty}{𝑒^{−𝑟^2/2𝜔_𝑠^2}𝑒^{−𝑟^2/2𝜔_𝑓^2}dr}\right|^2}{\displaystyle\int_{0}^{\infty}{\left|𝑒^{−𝑟^2/2𝜔_𝑠^2}\right|^2dr}\displaystyle\int_{0}^{\infty}{\left|𝑒^{−𝑟^2/2𝜔_𝑓^2}\right|^2dr}} \\
      &= \frac{\left|\displaystyle\int_{0}^{\infty}{𝑒^{−𝑟^2/2𝜔_𝑠^2−𝑟^2/2𝜔_𝑓^2}dr}\right|^2}{\displaystyle\int_{0}^{\infty}{\left|𝑒^{−𝑟^2/2𝜔_𝑠^2}\right|^2dr}\displaystyle\int_{0}^{\infty}{\left|𝑒^{−𝑟^2/2𝜔_𝑓^2}\right|^2dr}} \\
      \end{align*}$$ 

6. For a step-index SMF operating at $1550nm$ with the following parameters:   
        Core radius, $a$ $5\mu m$  
        Cladding index, $n_{cl}$ 1.46  
        Cut-off wavelength, $\lambda_c$ $1.24\mu m$  
    Calculate the spot size of the fibre @ 1550nm
    > $\dfrac{\omega}{a}=0.65+\dfrac{1.62}{V^3/2}+\dfrac{2.88}{V^6}$  
    > $V=ka\sqrt{n_{co}^2-n_{cl}^2}$ with $k=\dfrac{2\pi}{\lambda}$  
    > $\lambda_c = \dfrac{2\pi}{V_c}a\sqrt{n_{co}^2-n_{cl}^2}$ with $V_c = 2.405$  
    > $\to n_{co}\approx 1.463$ 
    > $\to V=1.924$ 
    > $\to \omega = 6.569\mu m$ 