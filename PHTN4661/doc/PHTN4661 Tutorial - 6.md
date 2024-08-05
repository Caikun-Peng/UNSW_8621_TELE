---
Owner: Peng, Caikun
Electives: Level 4
Last edited time: 2024-05-04
Course Progress: In Progress
Note Progress: In Progress
Note ID: PHTN4661-Tut-5
---

- Tutorial 6 Dispersion and bandwidth

1. What is dispersion in fibre optics? Explain briefly why dispersion is extremely important to optical fibre communication.
    > Dispersion in fibre optics refers to the phenomenon where the speed of light waves varies within the optical fibre based on their wavelength.  (Tutorial 5s, page 6)
    > $$D=-\dfrac{\lambda}{c}\dfrac{d^2n}{d\lambda^2}\qquad[ps/nm\cdot km]$$
    > Dispersion limits the bandwidth of the communication system.
1. What is phase velocity of an optical wave or signal? How we understand it from the field expression – phase part of optical wave in a uniform material or waveguide? Explain briefly, using an example, how it would influence optical signal propagation and behaviour in various applications.
    > The phase velocity of an optical wave or signal refers to the speed at which the phase of the wave propagates in space.  (Tutorial 5s, page 2)
    > $$V_p=\frac{\omega}{\beta}, \omega=2\pi f,\beta=\frac{2\pi}{\lambda}n$$
    > 
1. What is group velocity of an optical wave or signal? How we understand it from the field expression – amplitude part of optical wave in a uniform material or waveguide? Explain briefly how it would influence optical signal propagation and behaviour in various applications.
    > Group velocity is the speed at which the envelope of a wave packet or a pulse travels through a medium. This is especially important in optical communications because it is the velocity at which **information or energy** is conveyed along the fibre.
    > $$V_g = \frac{d\omega}{d\beta}$$
    > 
1. Please define and explain their differences: What is group velocity delay of an optical wave or signal? What is group velocity delay difference? What is group velocity dispersion (see next question)?  
    Please note: While the term GVD is frequently used in textbooks and references. GVD can mean group velocity delay in some cases and group velocity dispersion in other cases. In addition, see the question below, group velocity dispersion may be defined differently, with respect to $\omega$ and $\lambda$, respectively.
5. Please find and explain the different dispersions in different optical waveguides or fibres: 
    1. material dispersion
    2. modal dispersion or intermodal dispersion; 
    3. waveguide dispersion or intramodal dispersion 
    4. polarisation mode dispersion or PMD (Please search online by yourself)
6. Explain briefly the main advantages and disadvantages of single-mode fibres with respect to multimode optical fibres.
7. When transmitting in a uniform, dispersive material of refractive index $n(\lambda)$, the propagation constant of optical wave of wavelength $\lambda$ is $\beta = 2\pi n/\lambda$. The phase velocity and group velocity of optical wave are defined as $V_p = \omega/\beta$ and $V_g = d\omega/d\beta$ with angular frequency $\omega=2\pi f$, respectively.
    1. Show that $V_p = \omega/\beta = c / n$ and $V_g = d\omega/d\beta = c / (n - \lambda dn/d\lambda) = c / n_g$ with group index defined as $n_g = n - \lambda dn/d\lambda$. 
        > $$V_p=\frac{\omega}{\beta}=\frac{2\pi f}{2\pi n/\lambda} = \frac{\lambda f}{n} = \frac{\frac{c}{f}f}{n} = \frac{c}{n}$$
        > $$V_g=\frac{d\omega}{d\beta}=\frac{d\frac{2\pi c}{\lambda}}{d\frac{2\pi n}{\lambda}}=c\frac{d\frac{1}{\lambda}}{d\frac{n}{\lambda}}=c\frac{d\frac{1}{\lambda}/d\lambda}{d\frac{n}{\lambda}/d\lambda}=c\frac{-\frac{1}{\lambda^2}}{-\frac{n}{\lambda^2}+\frac{1}{\lambda}\frac{dn}{d\lambda}}=\frac{c}{n-\lambda dn/d\lambda}=\frac{c}{n_g}$$
    1. The group velocity dispersion (GVD) is defined as $\text{𝐆𝐕𝐃} = \dfrac{𝐝}{𝐝𝛚}\dfrac{𝟏}{𝐕_𝐠}$, i.e. GVD as the derivative of the inverse of group velocity of light in a material with respect to angular frequency $\omega$. Here GVD is defined as the group velocity delay difference per unit length per unit frequency and has the unit such as $[s^2 /m]$.  
        Show that in the case of optical wave transmitting in uniform material, $\text{GVD} = \dfrac{\lambda^3}{2\pi c^2}\dfrac{d^2n}{d\lambda^2}$.  
        $$\begin{align*}GVD
            &= \frac{d}{d\omega}\frac{1}{V_g}=\frac{d}{d\omega}\frac{d\beta}{d\omega}\\
            &= \frac{d}{d(\frac{2\pi c}{\lambda})}\frac{n-\lambda\frac{dn}{d\lambda}}{c}\\
            &=\frac{d(\frac{n-\lambda\frac{dn}{d\lambda}}{c})}{d\lambda}\frac{d\lambda}{d(\frac{2\pi c}{\lambda})}\\
            &= \left(\frac{d(\frac{n}{c})}{d\lambda}-\frac{d(\frac{\lambda dn}{c d\lambda})}{d\lambda}\right)\left(-\frac{\lambda^2}{2\pi c}\right)\\&= \left(\frac{dn}{c d\lambda} - \left(\frac{d(\frac{\lambda}{c})}{d\lambda}\frac{dn}{d\lambda}+\frac{\lambda}{c}\frac{d(\frac{dn}{d\lambda})}{d\lambda}\right)\right)\left(-\frac{\lambda^2}{2\pi c}\right)\\
            &= \left(\frac{dn}{c d\lambda} - \left(\frac{dn}{c d\lambda}+\frac{\lambda}{c}\frac{d^2n}{d\lambda^2}\right)\right)\left(-\frac{\lambda^2}{2\pi c}\right)\\
            &= \left(-\frac{\lambda}{c}\frac{d^2n}{d\lambda^2}\right)\left(-\frac{\lambda^2}{2\pi c}\right)\\
            &= \dfrac{\lambda^3}{2\pi c^2}\dfrac{d^2n}{d\lambda^2}
            \end{align*}$$
    1. Similarly the GVD parameter is usually defined as $\text{𝐃} = \dfrac{𝐝}{𝐝\lambda}\dfrac{𝟏}{𝐕_𝐠}$, $D$ is the derivative of the inverse of group velocity of light in a material with respect to wavelength $\lambda$. $\omega$. Here GVD is defined as the group velocity delay difference per unit length per unit wavelength and has the unit such as $[s/m^2]$.   
        Show that in the case of optical wave transmitting in uniform material, $𝐃 = − \dfrac{\lambda}{c}\dfrac{d^2n}{d\lambda^2}$.  
    
    Please note: D is used widely in engineering applications and we will use D instead GVD in most of tutorial questions.


8. The bandwidth $B$ of an optical fibre can be defined as $B = \dfrac{0.25}{σ}$ where $\sigma$ is the rms pulse broadening (due to factors such as material, modal or waveguide dispersion).
    1. Explain briefly why rms pulse broadening is used and how fibre length affects the bandwidth. 
    2. How to understand we have used the number of 0.25 here. What could be the issues if we use the number of 0.05 or 1.25 to replace 0.25.

    

9. A step index multimode (SI-MM) optical fibre has the following parameters:
    - core diameter = 62.5$\mu$m 
    - overall fibre diameter = 125$\mu$m 
    - core index = 1.48 
    - cladding index = 1.46 
    - length of fibre = 2 km 
    - fibre attenuation = 0.8 dB/km  
    
    An LED optical source has the following radiation pattern: $I(\theta) = I_0 \cos^4\theta$ where Io is the maximum emitting intensity. The LED emits rectangular optical pulses of $1ns$ width, at $\lambda = 1.55 μm$ with its spectral width is $S_\lambda= 30 nm$. The diameter of LED’s emitting area = $80\mu m$.
    1. Considering the material dispersion $D = 17 ps/nm/km$ at $\lambda = 1.55 μm,$ calculate the product of bandwidth - distance, i.e. $B\cdot L$, for this fibre. 
        > 
    1. If the LED is ideally butt-joined to the fibre, calculate the launching efficiency. 
        > 
    2. If the LED is used as the digital signal source over a 10 km link of the fibre, estimate the maximum possible data rate.

    [link](https://www.desmos.com/calculator/tbiv2y90fd)

2. For a commercial single-mode silica optical fibre operating at $\lambda = 1.55 μm$, with the material dispersion $D = 17 ps/nm/km$. This fibre has its cut-off wavelength at $\lambda_c = 1.26 μm$, its cladding index $n_2=1.46$, and its core radius $a=5μm$.
    1. If a LD of spectral width $S_\lambda= 0.01 nm$, is used as for light transmitter, estimate the value of bitrate - distance product, i.e. B$\cdot$L, for this fibre. 
        > 
    2. Calculate the maximum allowable bitrate over a $50 km$ link of the fibre.
        > 