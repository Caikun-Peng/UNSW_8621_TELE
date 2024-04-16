---
Owner: PPeng, Caikun
tags:
  - Level-5
Last edited time: 2024-02-21T13:32
Course Progress: Finished
Notes Progress: In progress
---
# Website

> [https://moodle.telt.unsw.edu.au/course/view.php?id=79549](https://moodle.telt.unsw.edu.au/course/view.php?id=79549)  

# Textbook

> [https://1drv.ms/b/s!AuXfaR2IFRyogSUuy8tDbeqst1eX?e=cbAFos](https://1drv.ms/b/s!AuXfaR2IFRyogSUuy8tDbeqst1eX?e=cbAFos)

# Instructor

|Professor| Office| Tel| Email|
|---|---|---|---|
|R. Ramer | EE 308| 9385 - 4759| ror@unsw.edu.au|

# Assessment Tasks

|Assessment|Weighting|Aligned CLOs|Due Date|Feedback Date|
|---|---|---|---|---|
|1. Mid-Exam|20%|CLOs 1-3|week 5|week 8|
|2. Assignment  <br>  <br>[TELE9755 Assignment](https://www.notion.so/TELE9755-Assignment-42cca3eab4d84bafa2a86b8fee1922bd?pvs=21)|20%|CLOs 1-3|week 8|week 10|
|3. Final Exam|60%|CLOs 1-4|exam timetable||

# Lectures

## Recapitulation of Transmission Lines Theory

![[2022_L1ADMIN_INTRO_tele9755_Stud_m.pdf]]

![[RECAP_TL123_t2_Students_m.pdf]]

![[L3Smith_Chart1_t2_students.pdf]]

![[RECAP_(3).pdf]]

### W1 INTRODUCTION TO RF / MICROWAVE ENGINEERING

### Microwave Region in Electromagnetic Spectrum

**Frequencies** between 3**00 MHz and 300 GHz**

**Wavelengths** from $\lambda=1m$﻿ to $\lambda=1mm$﻿

### What is so SPECIAL about RF / Microwave Engineering / Electronics?

**Standard circuit theory** is not valid at microwave frequencies

**Skin effect** occurs at microwave frequencies

In distributed circuits, **radiation** from circuit elements is present

### RF/Microwave Engineering vs Electromagnetic

**RF / Microwave engineering**  
results can be expressed in terms of simpler circuit theory such as power, impedance, voltage, current  

**Electromagnetic**  
find the electric and magnetic field, as functions of spatial coordinates.  

### Applications of RF/ Microwaves and Characteristics

The unique characteristics offered by the **high-frequency range**

- **More bandwidth**
- **More antenna gain**
- **Frequency reuse**
- Various molecular, atomic and nuclear resonances
- The effective reflection area of a radar target is proportional to the target’s  
    electrical size at microwave frequencies, thus establishing them as preferred for  
    radar systems  
    

### Wireless Basic Radio Transmitter/Receiver Block

![[Untitled 18.png|Untitled 18.png]]

![[Untitled 1 6.png|Untitled 1 6.png]]

### W1 RECAPITULATION OF TRANSMISSION LINES THEORY

### Lumped-element circuit model for a transmission line

### A transmission line

A transmission line is often schematically represented as a two-wire line.

![[Untitled 2 6.png|Untitled 2 6.png]]

The lumped element circuit model, where R, L, G, C are per unit length quantities.  
(Combined R, L, C for both conductors)  

![[Untitled 3 5.png|Untitled 3 5.png]]

![[Untitled 4 5.png|Untitled 4 5.png]]

Where R, L, G, C are per unit length quantities and depend on

- Geometric parameters, and
- Electromagnetic constitutive parameters:
    - $\mu_c$﻿ = magnetic permeability of conductors
    - $\sigma_c$﻿= electric conductivity of conductors
    - $\varepsilon$﻿= electrical permittivity of conductors
    - $\mu$﻿= magnetic permeability of dielectrics
    - $\sigma$﻿= electric conductivity of dielectrics

### Telegrapher’s equation

$\frac{d^2V(z)}{dz^2}-\gamma^2V(z)=0$

General solution

$V(z)=V_O^+e^{-\gamma z}+V_O^-e^{\gamma z}$

$\gamma=\sqrt{(R+j\omega L)(G+j\omega C)}=\alpha+j\beta$﻿

$\gamma $﻿ Complex propagation constant (coefficient)

$\alpha $﻿ Attenuation constant in $dB/m$﻿

$\beta$﻿ Phase (propagation) constant in $rad/m$﻿, $\beta=2\pi/\lambda$﻿

$e^{-\gamma z}$﻿ factor represents wave propagation in $+z$﻿ direction

$e^{\gamma z}$﻿ factor represents wave propagation in $-z$﻿ direction

### Characteristic impedance of the transmission line

$Z_0=\frac{R+j\omega L}{\gamma}=\sqrt{\frac{R+j\omega L}{G+j\omega C}}=\frac{V_O^+}{I_O^+}=-\frac{V_O^-}{I_O^-}$

  

### Lossless Transmission Line

Conditions: $\alpha=0,\ R=0,\ G=0$﻿

- propagation constant
    
    $\gamma=j\omega\sqrt{LC}$﻿, $\beta=\omega\sqrt{LC}=2\pi/\lambda$﻿
    
- Characteristic impedance
    
    $Z_0=\sqrt{L/C}$﻿
    
- Phase velocity
    
    $v_p=\omega/\beta=1/\sqrt{LC}$﻿
    
- Wavelength
    
    $\lambda=2\pi/\beta=2\pi/\omega\sqrt{LC}=v/f $﻿
    
- Electrical length
    
    $\theta=\beta l=(2\pi/\lambda)l$﻿
    

### Voltage reflection coefficient

$\begin{aligned}$

  

$\Gamma=|\Gamma|e^{j\theta_r}$﻿

### Observations for the load

- Matched load
    
    $Z_L=\infty;\ \Gamma=0;\ V_O^-=0$﻿
    

  

- Open circuit
    
    $Z_L=\infty;\ \Gamma=1;\ V_O^-=V_O^+$﻿
    

- Short circuit
    
    $Z_L=\infty;\ \Gamma=-1;\ V_O^-=-V_O^+$﻿
    

### Power (time average) delivered at the load

$\begin{aligned}$

### Return Loss

$RL=-20log|\Gamma|$﻿

### Insertion Loss

$IL=-20log|T|=-20log|1+\Gamma|$﻿

### Standing Waves

$V(z)=V_O^+[e^{-j\beta z}+\Gamma e^{j\beta z}]$﻿

if matched, $|V(z)|=|V_O^+|$﻿, derive the expression:

$\begin{aligned}$

The maximum voltage $|V_{max}|=|V_O^+|\cdot(1+|\Gamma|)$﻿

  

The minimum voltage $|V_{min}|=|V_O^+|\cdot(1-|\Gamma|)$﻿

### VSWR or SWR or S

The ratio of $V_{max}$﻿ to $V_{min}$﻿ is called the voltage standing wave ratio (VSWR), or, standing wave ratio (SWR or S)

$VSWR=SWR=S\triangleq\frac{V_{max}}{V_{min}}=\frac{1+|\Gamma|}{1-|\Gamma|}$

  

### NOT take notes

### Impedance Input

### Input Admittance of Lossless Line

### Half Wavelength Long Lossless Transmission Line

$Z_{in}=Z_L$﻿, half-wave L.L.T. do not modify the load impedance

- Prove
    
    $\begin{aligned}$
    

### Quarter-Wavelength Long Transmission Line

$Z_{in}=\frac{Z_O^2}{Z_L}$

  

  

### W2 Smith Chart

Smith Chart is a polar plot of the **voltage reflection coefficient**

It is not hard to using Smith Chart

$z_{in}=\frac{Z_{in}}{Z_0},\ \ z_L=\frac{Z_{L}}{Z_0}$

Wavelength scales cover a range from 0 to 0.5$\lambda$﻿

  

### W2 The Slotted Line

an instrument used to measure the unknown impedance of a load $Z_L$﻿

## Analysis of Microwave Networks

![[m_MwNA_1_MatrRepImAdSc_matr_1_2021_Students.pdf]]

![[m_MwNA_4_ANAL.pdf]]

![[m_MwNA_2_Genparam__2.pdf]]

![[1MwNA_6_2021_m.pdf]]

![[m_MwNA_3_ABCDmatrix___3.pdf]]

### W3 Impedance and Admittance Matrices

The total voltages and currents at z = 0:

$\begin{aligned}$

- **The impedance matrix:**
    
    $[V]=[Z][I]\\$
    

The impedance and admittance matrix are the reciprocals of each  
other:  

$[Y]=[Z]^{-1}$

- **The admittance matrix:**
    
    $[V]=[Y][I]\\$
    

Networks can be classified as:

**RECIPROCAL** (symmetrical):

$Z_{ij}=Z_{ji}\text{ and }Y_{ij}=Y_{ji}$﻿

**LOSSLESS**:

$Z_{ij},Y_{ij}$﻿ must be purely imaginary

  

### Equivalent Circuits for Two-Port Networks

![[Untitled 5 5.png|Untitled 5 5.png]]

(a) $T$﻿ equivalent

  

(b) $\pi$﻿ equivalent

### W3 Scattering Matrix

relating the amplitudes of the voltage wave incident on the ports $V_n^+$﻿ to the reflected one $V_n^-$﻿ from the ports

$|V^-|=[S]|V^+|$

$\begin{gathered}$

$S_{ij}=\frac{V_i^-}{V_j^+}\bigg|_{V_k^+=0,\ for \ k\neq j}$

  

Relation between [S] and [Z]

$([Z]-[U])[V^+]=([Z]+[U])[V^-]$

$[S]=\frac{V^-}{V^+}=\frac{[Z]-[U]}{[Z]+[U]}$

  

Characteristics of the Scattering Matrix

For **reciprocal networks:**

$S_{ij}=S_{ji}\text{ or }[S]=[S]^t$﻿

For **lossless networks:**

$[S]^t\cdot[S]^*=[U]\text{ or }[S]^*=\{[S]^t\}^{-1}$﻿

In summation form:

$\begin{gathered}$

  

  

### S-Matrix for a Two-Port Network

![[Untitled 6 4.png|Untitled 6 4.png]]

$\begin{gathered}$

- When port 2 is matched
    
    $Z_L=Z_0,\ \Gamma_L=\frac{V_2^+}{V_2^-}=0,\Rightarrow V_2^+=0$
    
    The reflection coefficient at port 1: $S_{11}=\frac{V_1^-}{V_1^+}$﻿
    
    The transmission coefficient: $S_{21}=\frac{V_2^-}{V_1^+}$﻿
    

For **reciprocal networks:**

$S_{12}=S_{21}$﻿

For **lossless networks:**

$|S_{11}|^2+|S_{21}|^2=1$﻿

### W3 ABCD Matrix

$V_1=AV_2+BI_2\\I_1=CV_2+DI_2$

$\begin{gathered}$

$\begin{gathered}$

the multiplication of each ABCD matrix belonging to the two-port networks should be performed in the same order

- Six of the most common circuit configurations in terms of ABCD two-port network representations
    
    ![[Untitled 7 3.png|Untitled 7 3.png]]
    
    ![[Untitled 8 3.png|Untitled 8 3.png]]
    
      
    
- Conversions Between Two-port Network Parameters
    
    ![[Untitled 9 3.png|Untitled 9 3.png]]
    
    ![[Untitled 10 3.png|Untitled 10 3.png]]
    
    $\begin{array}{l}$
    

### W3 Analysis of a 2-port Network Using S-Matrixl

### ‘EXTEND’ the PORTS

- For $z=0$﻿
    
    $\begin{gathered}$
    

  

- For $z=-l$﻿
    
    $\begin{aligned}$
    

### Symmetry Property

![[Untitled 11 3.png|Untitled 11 3.png]]

The symmetry of the network can be used to simplify the analysis

Can divide this network into two identical halves and analyze one half of  
the circuit  

With an electric wall termination  
(i.e. a short circuit;  
$\vec{E}$﻿ field $\bot$﻿ on the wall):

![[Untitled 12 3.png|Untitled 12 3.png]]

  

With a magnetic wall termination  
(i.e. an open circuit;  
$\vec{E}$﻿ field tangential on the wall):

![[Untitled 13 3.png|Untitled 13 3.png]]

  

$S_{11}=\frac{1}{2}\left(S_e+S_m\right)=S_{22}\ \ \& \ \ S_{12}=\frac{1}{2}\left(S_e-S_m\right)=S_{22}$

  

An example:

![[Untitled 14 3.png|Untitled 14 3.png]]

$S_e=\frac{\left(Z_A\parallel\frac{1}{2}Z_B\right)-Z_0}{\left(Z_A\parallel\frac{1}{2}Z_B\right)+Z_0}$

$S_m=\frac{Z_A-Z_0}{Z_A+Z_0}$

### W4 PC matrix

Step 1:

a) IDENTIFY the EXTERNAL PORTS ‘P’ and INTERNAL PORTS ‘C’.

b) IDENTIFY the incident and reflected voltages:

$(V_P^+,V_P^-)$﻿ for all the external P ports

$(V_C^+,V_C^-)$﻿ for all the external C ports

Step 2:

$\begin{bmatrix}$

Step 3:

FIND the connection matrix $\Gamma$﻿, which relates the internal ports  
to each other; i.e. it relates  
$V_C^-$﻿ to $V_C^+$﻿:

$V_C^-$﻿$=\Gamma$﻿$V_C^+$﻿

  

Step 4:

CALCULATE the SCATTERING MATRIX of the network $\begin{bmatrix}$﻿, that relates $V_P^-$﻿ to $V_P^+$﻿:

$V_P^-=\left[S^P\right]V_P^+$﻿

$S^P=S_{PP}+S_{PC}\left[\Gamma-S_{CC}\right]^{-1}S_{CP}$﻿

## Transmission Line Technologies

![[TLsTechns_1_Summary.pdf]]

![[TLsTechns_2_INDUCTANCECAP.pdf]]

![[TLsTechns_3_resonators_1.pdf]]

![[TLsTechns_4_resonators_2.pdf]]

### W4 Summary of Transmission Lines Technologies & Microstrip line equations

For all Transmission lines we need to know  
propagation constant (coefficient) β and  
characteristic (wave) impedance  
$Z_O$﻿ , $Z_{TE}$﻿ , etc

### Coaxial Transmission Line

- The dominant mode of propagation is TEM.
- For the Co-Ax line: $\beta=\omega\sqrt{\mu_0\varepsilon_0\varepsilon_r}$﻿
- Co-Ax still works at DC.
- Used for long-distance, under the ocean, since there is no dispersion, only attenuation.
- The phase velocity $v_p=\omega/\beta$﻿ is not frequency-dependent

![[Untitled 15 3.png|Untitled 15 3.png]]

### WAVEGUIDES - Metallic tubes

Rectangular waveguide

![[Untitled 16 3.png|Untitled 16 3.png]]

Circular waveguide

![[Untitled 17 2.png|Untitled 17 2.png]]

![[Untitled 18 2.png|Untitled 18 2.png]]

a linear function of frequency

![[Untitled 19.png]]

### PLANAR TRANSMISSION LINES

![[Untitled 20.png]]

  

### W5 Implementation of Inductances and Capacitances at RF/Microwave Frequency

### TRANSMISSION LINES

![[Untitled 21.png]]

![[Untitled 22.png]]

![[Untitled 23.png]]

  

### LUMPED ELEMENTS

![[Untitled 24.png]]

### DISCONTINUITIES IN TRANSMISSION LINES

The most popular way to realize L and C.

- The gap between two TLs
    
    ![[Untitled 25.png]]
    
- Discontinuity on the outer conductor of a Coax
    
    ![[Untitled 26.png]]
    

  

- Open-End and its electrical model
    
    ![[Untitled 27.png]]
    
    ![[Untitled 28.png]]
    
- Bends (right angles etc.) and electrical model
    
    ![[Untitled 29.png]]
    
- Step Change in Width and its electrical model
    
    ![[Untitled 30.png]]
    
- T- junctions and their electrical model
    
    ![[Untitled 31.png]]
    

- Exercise
    
    ![[Untitled 32.png]]
    

- Solution
    
    ![[Untitled 33.png]]
    

### W5 MICROWAVE RESONATORS

### MW RESONATORS CONSIDERATIONS and CONFIGURATIONS

A resonator is an element capable of storing frequency-dependent  
electric and magnetic energy.  

The primary design considerations

- Size
    
    Resonators can take various forms and shapes at microwave frequencies.
    
- Resonant frequency
    
    the frequency at which the energy stored in the electric field equals the energy stored in the magnetic field. It is determined by the physical characteristics of the structure and dimensions.
    
- Unloaded Q
    
    the inherent loss in the resonator
    
- Spurious performance
    
    determined by how close the neighbouring resonant modes are to the operating mode
    
- Power handling.

Frequency dependant on size, as size $\downarrow, \Rightarrow f_o\uparrow$﻿

Q depends on Insertion Loss, as $Q\uparrow, \Rightarrow IL\downarrow$﻿

if $R=0$﻿, then $Q=\infty$﻿ (lossless)

### SERIES and PARALLEL RESONANT RLC CIRCUITS

- Parallel Resonant Circuit
    
    ![[Untitled 34.png]]
    
    The input impedance
    
    $\frac{1}{Z_{in}}=\frac 1 R + \frac 1 {j\omega L}+j\omega C$
    
    The complex power delivered to the resonator
    
    $\begin{align*}P_{in}&=\frac 1 2 VI^* = \frac 1 2 Z_{in}|I|^2 = \frac 1 2 |V|^2\frac 1 {Z_{in}^*}\\$
    
    the complex power written as
    
    $P_{in}=P_{loss}+2j\omega(W_m-W_e)$
    
    When $W_e = W_m \Rightarrow P_{in}=P_{loss}$﻿
    
    the resonant frequency
    
    $\omega_0 \dot{=} \frac 1 {\sqrt{LC}}$
    
    The power dissipated by the resistor R is
    
    $P_{loss}=\frac 1 2 \frac{|V|^2} R$
    
    The average electric energy stored in an electric field (in a capacitor C) is:
    
    $W_e=\frac 1 4 |V|^2C$
    
    The average magnetic energy stored in the magnetic field (in the inductor L) is:
    
    $W_m=\frac 1 4 |I_L|^2L=\frac 1 4 |V|^2\frac 1 {\omega^2L}$
    
      
    
    Near resonance, (i.e. $\omega=\omega_0+\Delta\omega$﻿, with $\Delta\omega$﻿ very small) the input impedance of a parallel resonant circuit can be approximated to:
    
    $Z_{in}=\frac 1 {\tfrac 1 R +2j\Delta\omega C}$
    
- Series Resonant Circuit
    
    ![[Untitled 35.png]]
    
    Input impedance $Z_{in}$﻿ for an RLC series circuit is:
    
    $Z_{in}=R+j\omega L+\frac 1 {j\omega C}$
    
    The complex power delivered to the resonator is
    
    $\begin{align*}P_{in}&=\frac 1 2 VI^* = \frac 1 2 Z_{in}|I|^2 = \frac 1 2 Z_{in}\left|\frac V {Z_{in}}\right|^2\\$
    
    the complex power written as
    
    $P_{in}=P_{loss}+2j\omega(W_m-W_e)$
    
    The input impedance becomes
    
    $Z_{in}=\frac {2P_{in}}{|I|^2}=\frac {P_{loss}+2j\omega(W_m-W_e)}{\dfrac 1 2 |I|^2}$
    
    When $W_e = W_m \Rightarrow P_{in}=P_{loss}$﻿
    
    the resonant frequency
    
    $\omega_0 \dot{=} \frac 1 {\sqrt{LC}}$
    
    The power dissipated by the resistor R is
    
    $P_{loss}=\frac 1 2|I|^2R$
    
    The average electric energy stored in an electric field (in a capacitor C) is:
    
    $W_e=\frac 1 4 |V|^2C=\frac 1 4 |I|^2\frac 1 {\omega^2 C}$
    
    The average magnetic energy stored in the magnetic field (in the inductor L) is:
    
    $W_m=\frac 1 4 |I|^2 L$
    
- Quality Factor
    
    Quality factor (Q) is a measure of the inherent loss of a resonant circuit;  
    lower loss implies higher Q.  
    
    $Q\dot{=}\omega_0\left(\frac{\text{energy\ stored}}{\text{energy loss/cycle}}\right)=\omega_0\left(\frac{W_m+W_e}{P_{loss}}\right)=\omega_0\frac {2W_m}{P_{loss}}=\omega_0\frac {2W_e}{P_{loss}}$
    
    For Parallel Resonance
    
    $Q=\omega_0\frac {2W_m}{P_{loss}}=\frac R {\omega_0L}=\omega_0RC$
    
    Input impedance
    
    $Z_{in}\simeq\frac R {1+j2Q\dfrac{\Delta\omega}{\omega_0}}$
    
    For Serial Resonance
    
    $Q=\frac{\omega_0L} R=\frac 1 {\omega_0RC}$
    
    Input impedance
    
    $Z_{in}\simeq R+\frac{2RQ\Delta\omega}{\omega_0}$
    
- Results for Series and Parallel Resonators
    
    ![[Untitled 36.png]]
    

### Transmission Line Resonators

Open and short-circuited TLs segments with certain lengths are used to form resonators.

For 1/4 $\lambda $﻿ Transmission Line

![[Untitled 37.png]]

![[Untitled 38.png]]

For 1/2 $\lambda$﻿ Transmission Line

![[Untitled 39.png]]

![[Untitled 40.png]]

$Z_{in}=R=\frac{Z_0}{\alpha l}$

### CALCULATION of RESONANT FREQUENCY

- Resonant Frequency of Conventional Transmission Line Resonators
    
    At resonance at any point on the transmission line, the sum of the input impedance (admittance) seen looking at either side must be zero.
    
    $Z_{in}^r(x)+Z_{in}^l(x)=0$
    
    Consider a lossless TL terminated in a short circuit at both ends.
    
    ![[Untitled 41.png]]
    
    At resonance $Z_1+Z_2=0$﻿, where $Z_1=jZ_0\tan{\beta l_1}$﻿ and $Z_2=jZ_0\tan{\beta l_2}$﻿.
    
    Then $j\tan{\beta l_1}=-j\tan{\beta l_2}$﻿
    
    Or $\beta l_1=-\beta l_2+q\pi \Rightarrow \beta(l_1+l_2)=\beta l =\dfrac{2\pi}{\lambda}l\equiv q\pi$﻿, where $q=1,2,3...$﻿
    
    Therefore, $l=q\dfrac \lambda 2$﻿ or $\lambda = \dfrac{2 l}{q}$﻿.
    
    $\lambda_0=\dfrac v f=\dfrac c {f\sqrt{\varepsilon_r}}\equiv \dfrac{2l}q$﻿.
    
- Resonant Frequency Calculation Using Transverse Resonance Technique
    
    Transverse Resonance Technique enables us to calculate the resonance frequency of any structure.
    
    A microstrip TL resonator loaded with a rectangular strip along the length of the resonator:
    
    ![[Untitled 42.png]]
    
    ![[Untitled 43.png]]
    
    $\Gamma'_L =\Gamma_{Lo.c.}e^{-2j\beta l_2}=e^{-2j\beta l_2} $﻿
    
    $\Gamma_{in}=\dfrac {V_1^-} {V_1^+}=S_{11}+\dfrac{S_{12}\Gamma'_LS_{21}}{1-\Gamma'_LS_{22}}=S_{11}+\dfrac{S_{12}e^{-2j\beta l_2}S_{21}}{1-e^{-2j\beta l_2}S_{22}}$﻿
    
    $\Gamma'_{in}=\dfrac {{V_1^-}'} {{V_1^+}'}=\dfrac{V_1^-e^{-j\beta l_1}}{V_1^+e^{+j\beta l_1}}=\dfrac{V_1^-}{V_1^+}e^{-2j\beta l_1}\text{ and }(\equiv\Gamma_{in}e^{-2j\beta l_1})$﻿
    
    ……
    

## Microwave Filters

![[filters-Lecture1_2020_tele9755_m.pdf]]

![[filters-Lecture2_T2_2022_m.pdf]]

![[filters-Part4_DesignExampleAlone_m.pdf]]

### W6 Basic Principles

- FILTER DESIGN USING INSERTION LOSS METHOD
    
    ![[Untitled 44.png]]
    
    $P_L=P_i\left[1-|\Gamma_{in}(\omega)|^2\right]$﻿
    
    $P_{LR}=\dfrac{\text{Power Available from Source}}{\text{Power Delivered to Load}}=\dfrac{P_i}{P_L}=\dfrac 1 {1-|\Gamma_{in}(\omega)|^2}$﻿ and $IL=10\log P_{LR}(dB)$﻿
    
    - MAXIMALLY FLAT FILTER RESPONSE (Butterworth response)
        
        $P_{LR}=1+k^2\left(\dfrac \omega {\omega_C} \right)^{2N}$﻿, where $N $﻿ is the order of the filter, $\omega_C$﻿ is the cut off frequency.
        
        ![[Untitled 45.png]]
        
    - EQUAL RIPLE RESPONSE (Chebyshev Response)
        
        $P_{LR}=1+k^2T_N^2\left(\dfrac{\omega}{\omega_C}\right)$﻿, where $T_N$﻿ is the coefficient, representing Chebyshev Polynomial.
        
        - Chebyshev Polynomial $T (x)$﻿
            
            $T_N(x)=\cos(N\cos^{-1}x)\text{ for } |x|<1$﻿  
            When  
              
            $N=0;\ T_0(x)=1.\\ N=1;\ T_1(x)=x.$﻿
            
        
        ![[Untitled 46.png]]
        
    - ELLIPTIC RESPONSE (Cauer Response)
        
          
        
        ![[Untitled 47.png]]
        
    - Plotting both Butterworth and Chebyshev filter responses together
        
        ![[Untitled 48.png]]
        
        At high frequency when $\omega \gg\omega_C$﻿:
        
        For Butterworth filter:
        
        $P_{LR}=k^2\left(\frac{\omega}{\omega_C}\right)^{2N}$
        
        For Chebychev filter:
        
        $P_{LR}=\frac{K^2}4\left(\frac{2\omega}{\omega_C}\right)^{2N}$
        
        For the same N, Chebyshev response yields a higher rejection out of band (property that is desirable in filters)
        
- FILTER TRANSFORMATION
    - Intro
        - Impedance scaling
            
            If $Z_0=R_0$﻿, the new scaled filter component values as $L',\ C',\ R_S',\ R_L'$﻿ are given by:
            
            $L'=R_0L;\ C'=\dfrac C{R_0};\ R_L'=R_0R_L;\ R_S'=R_0 .$﻿
            
        - Frequency Scaling
            
            If $\omega\neq1$﻿, then $\omega\to\dfrac{\omega}{\omega_C}$﻿
            
            Then $jX_k=j\dfrac{\omega}{\omega_C}L_k=j\omega L_k',\ jB_k=j\dfrac{\omega}{\omega_C}C_k=j\omega C_k'.$﻿
            
            The new elements are
            
            $L_k'=\dfrac{L_k}{\omega_C};\ C_k'=\dfrac{C_k}{\omega_C}.$﻿
            
        - When both impedance and frequency scaling are needed
            
            $L_k'=\dfrac{R_oL_k}{\omega_C};\ C_k'=\dfrac{C_k}{R_0\omega_C}.$﻿
            
    - Low-Pass Filter to High-Pass Filter Transformation
        
        To covert a low-pass filter to a high-pass filter response, we need to do a frequency transformation.
        
        $\omega\to-\dfrac{\omega_C}{\omega}$﻿, therefore
        
        $jX_k=-j\dfrac{\omega_C}{\omega}L_k=\dfrac{1}{j\omega C_k'}$﻿ and
        
        $jB_k=-j\dfrac{\omega_C}{\omega}C_k=\dfrac 1 {j\omega L_k'}$﻿
        
        series inductors $L_k$﻿ must be replaced with capacitors $C ' _k$﻿,
        
        shunt capacitors $C_k$﻿ must be replaced with inductors $L_k'$﻿.
        
        The new components values are:
        
        $C_k'=\dfrac{1}{\omega_CL_k};\ L_k'=\dfrac{1}{\omega_CC_k}.$﻿
        
    - Low-Pass Filter to Band-Pass Filter Transformation
        - Frequency transformation:
            
            $\begin{align*}$
            
            $\omega_2,\ \omega_1$﻿
            
            denote the edges of the pass band
            
            $\Delta=\dfrac{\omega_2-\omega_1}{\omega_0}$﻿
            
            fractional bandwidth of the passband
            
            $\omega_0 = \sqrt{\omega_1\omega_2}$﻿
            
            the central frequency
            
            ![[Untitled 49.png]]
            
            $\begin{align*}$
            
              
            
        - Impedance transformation:
            - For inductance:
                
                ![[Untitled 50.png]]
                
                $\begin{align*}$
                
            - For capacitor, similarly:
                
                ![[Untitled 51.png]]
                
                $\begin{align*}$
                
    - Table Prototype Filter Transformation
        
        ![[Untitled 52.png]]
        
- Example
    
    in Lecture\#1
    

### W7 Realization of Microwave Filters

- Recap:
    
    Input impedance $Z_{in}=Z_0\left(\dfrac{Z_L+jZ_0\tan{\beta l}}{Z_0+jZ_L\tan{\beta l}}\right)$﻿
    
    For a short-circuited transmission line ($Z_L=0$﻿), the input impedance is
    
    $Z_{in}=jZ_0\tan{\beta l}$﻿
    
    For an open-circuited T.L.,
    
    $Z_{in}=-jZ_0\cot{\beta l}=-j\dfrac{Z_0}{\tan{\beta l}}$﻿, and $Y_{in}=jB=jY_0\tan{\beta l}$﻿
    
    For Quarter-wave T.L.:
    
    $\tan{\beta l}=\tan{\left(\dfrac{ 2\pi}{\lambda}\dfrac \lambda 4 \right)}=\tan{\dfrac \pi 2}\to\infty$﻿
    
    $Z_{in}=Z_0\left(\dfrac{Z_L+jZ_0\tan{\beta l}}{Z_0+jZ_L\tan{\beta l}}\right)=Z_0\dfrac{\tan{\beta l}}{\tan{\beta l}}\left(\dfrac{\dfrac{Z_L}{\tan{\beta l}}+jZ_0}{\dfrac{Z_0}{\tan{\beta l}}+jZ_L}\right)=Z_0\left(\dfrac{\dfrac{Z_L}{\infty}+jZ_0}{\dfrac{Z_0}{\infty}+jZ_L}\right)=\dfrac{Z_0^2}{Z_L}$﻿
    
    ![[Untitled 53.png]]
    
    - Microwave Filter Design - STEPS
        
        Determine the appropriate number of filter elements for the required frequency response
        
        Draw the ladder circuit either starting with a series or shunt element
        
        Perform the impedance/frequency scaling and frequency transformation
        
        Replace the lump elements with distributed short-circuited or open-circuited stubs
        
- **REALISATION OF FILTERS**
    - LOW-PASS FILTERS USING TRANSMISSION LINE STUBS
        - Richard’s Transformation
            
            ![[Untitled 54.png]]
            
            maps $\omega $﻿ plane to the $\Omega$﻿ plane:
            
            $\Omega = \tan{\beta l}=\tan{\dfrac{\omega l}{v_p}}$﻿
            
            the reactance of an inductor becomes
            
            $jX_L=j\omega L\to j\Omega L=jL\tan{\beta l}$﻿
            
            $(Z_{in}^{SC}=jZ_0\tan{\beta l})$﻿
            
            and the susceptance of a capacitor becomes
            
            $jB_C=j\omega C\to j\Omega C=jC\tan{\beta l}$﻿
            
            $(Y_{in}^{OC}=jB=jY_0\tan{\beta l})$﻿
            
            To obtain the same unity frequency, $\omega=\Omega=1$﻿
            
            $\Omega=1=\tan{\beta l}$﻿
            
            the stub length must be of $l=\lambda/8$﻿
            
        - Kuroda’s Identities
            
            ![[Untitled 55.png]]
            
            Each box represents a ‘unit element’ or a transmission line of indicated impedance  
            and length  
            $l=\lambda/8\ at\ \omega_c$﻿
            
    - STEPPED IMPEDANCE LOW-PASS FILTER
        
        ![[Untitled 56.png]]
        
        - Approximate Equivalent Circuits for Short Transmission Line Sections
            
            ![[Untitled 57.png]]
            
            ![[Untitled 58.png]]
            
            If the characteristic impedance of the T.L., $Z_0$﻿ is very high and T.L. is short $(\beta l<\dfrac \pi 4 )$﻿.
            
            $\Rightarrow\ X\cong Z_0\beta l\ \&\ B\approx0\ (\tan{\beta l }\cong\beta l) $﻿
            
            ![[Untitled 59.png]]
            
            the high impedance T.L. corresponds to series inductor
            
            Short length + narrow $\Rightarrow$﻿ inductor.
            
            If the characteristic impedance of T.L. $Z_0$﻿ is very small, and the T.L. is short.
            
            $\Rightarrow\ X\cong0\ \&\ B\approx Y_0\beta l$﻿
            
            If a T.L. that has a low impedance & short length it is equivalent to a shunt capacitor
            
            ![[Untitled 60.png]]
            
            Short length + wide $\Rightarrow$﻿ represents a shunt capacitor
            
            For inductor: $\beta l=\dfrac{LR_0}{Z_h}$﻿
            
            For capacitor: $\beta l = \dfrac{CZ_l}{R_0}$﻿
            
    - REALIZATION of BAND-PASS FILTERS
        
          
        

### W7 Examples of Common Filter Design

  

## Microwave Amplifier Design

### TWO-PORT POWER GAINS

![[Untitled 61.png]]

- The reflection coefficient:
    
    $\Gamma_S=\dfrac{Z_S-Z_0}{Z_S+Z_0},\ \Gamma_L=\dfrac{Z_L-Z_0}{Z_L+Z_0},\ $﻿
    
    $\Gamma_{in}=\dfrac{V_1^-}{V_1^+}=S_{11}+\dfrac{S_{12}\Gamma_LS_{21}}{1-S_{22}\Gamma_L}=\dfrac{Z_{in}-Z_0}{Z_{in}+Z_0}$﻿
    
    $\Gamma_{out}=\dfrac{V_2^-}{V_2^+}=S_{22}+\dfrac{S_{12}\Gamma_SS_{21}}{1-S_{11}\Gamma_S}=\dfrac{Z_{out}-Z_0}{Z_{out}+Z_0}$﻿
    
- Gain:
    
    Power Gain: $G=\dfrac{P_L}{P_{in}}$﻿
    
    Available Gain: $G_A=\dfrac{P_{avn}}{P_{avs}}=\dfrac{power\ available\ from\ network}{power\ available\ from\ source}$﻿
    
    Transducer Gain: $G_T=\dfrac{P_L}{P_{avs}}$﻿
    
    (A set of derivation)
    
    $G_T=\underbrace{\dfrac{1-|\Gamma_S|^2}{|1-\Gamma_{in}\Gamma_S|}}_{G_S}\cdot\underbrace{|S_{21}|^2}_{G_0}\cdot\underbrace{\dfrac{1-|\Gamma_L|^2}{|1-S_{22}\Gamma_L|^2}}_{G_L}$
    
    $G_S$﻿ and $G_L$﻿ are due to the impedance matching of the transistor to the impedance $Z_0$﻿
    

### STABILITY OF AMPLIFIERS

- UNILATERAL
    
    $S_{12}\to0$﻿
    
    When $S_{12}\to0$﻿,
    
    $|\Gamma_{in}|=|S_{11}|<1\ \&\ |\Gamma_{out}|=|S_{22}|<1$﻿
    
    $\Rightarrow$﻿ unconditional stability
    
- BILATERAL
    
    $|\Gamma_{in}|<1\Rightarrow Stable$﻿
    
    $|\Gamma_{in}|>1\Rightarrow Unstable$﻿
    
    $|\Gamma_{in}|=1\Rightarrow Border$﻿
    
    use **stability circles**
    
    Output stability circle
    
    $C_L=\dfrac{(S_{22}-\Delta S_{11}^*)^*}{|S_{22}|^2-|\Delta|^2}$﻿
    
    $R_L=\left|\dfrac{S_{12}S_{21}}{|S_{22}|^2-|\Delta|^2}\right|$﻿
    
    $\Delta=S_{11}S_{22}-S_{12}S_{21}$﻿
    
    ![[Untitled 62.png]]
    
    Input stability circle
    
    $C_S=\dfrac{(S_{11}-\Delta S_{22}^*)^*}{|S_{11}|^2-|\Delta|^2}$﻿
    
    $R_S=\left|\dfrac{S_{12}S_{21}}{|S_{11}|^2-|\Delta|^2}\right|$﻿
    
    $\Delta=S_{11}S_{22}-S_{12}S_{21}$﻿
    
    ![[Untitled 63.png]]
    
- A TEST FOR UNCONDITIONALLY STABLE CASE
    
    $\begin{align*}$
    
      
    
      
    

## Power Dividers and Directional Couplers

# Tutorial

### Tutorial 1

![[Tut1-Qs.pdf]]

1. The current on a transmission line is given as $i(t)=1.2cos(1.51*10^{10} t-80.3z)$﻿.  
    Determine  
    a) the frequency,  
    b) the wavelength,  
    c) the phase velocity  
    d) the phasor representation of the current.  
    

- Solution
    
    $i(t)=Acos(ft+\beta z),\ \beta=2\pi/\lambda$﻿
    
    $\omega=2\pi f\to f=2.4GHz$﻿
    
    $\lambda=2\pi/\beta= 2π / 80.3 ≈ 0.0785\ m$﻿
    
    $v_p = \omega/\beta=f * λ = (1.51 * 10^10 Hz) * (0.0785 m) ≈ 1.1865 * 10^9 m/s$﻿
    
    $i=A∠\beta=1.2∠-80.3\degree$﻿
    

1. A transmission line has the following per unit length parameters:  
    L= 0.2uH/m , C= 300pF/m, R= 5Ω/m and G= 0.01S/m.  
    Calculate  
    the complex propagation constant and  
    the characteristic impedance of this line at 500MHz.  
    Re-calculate these quantities in the absence of loss (R G= = 0).  
    

- Solution
    1. Complex Propagation Constant ($γ$﻿):  
          
        $γ = \sqrt{(R + jωL)(G + jωC)},\ \omega=2\pi f$﻿
    2. Characteristic Impedance ($Z_0$﻿):  
          
        $Z_0 = \sqrt{((R + jωL) / (G + jωC))}$﻿

1. A lossless transmission line of electrical length $l=0.3λ$﻿ and characteristic impedance $Z_O =75 Ω$﻿ is terminated with a complex load impedance $Z_L= ( 40+j20 )Ω$﻿ .  
    Find  
    the reflection coefficient at the load,  
    the SWR on the line and  
    the input impedance to the line.  
    

- Solution
    1. Reflection Coefficient at the Load ($Γ_L$﻿):  
          
        $Γ_L = (Z_L - Z_0) / (Z_L + Z_0)$﻿
    2. Standing Wave Ratio (SWR):  
        SWR  
        $= (1 + |Γ_L|) / (1 - |Γ_L|)$﻿
    3. Input Impedance to the Line ($Z_{in}$﻿):  
          
        $Z_{in} = Z_0 * (Z_L + jZ_0 * tan(βl)) / (Z_0 + jZ_L * tan(βl))$﻿

1. A 100Ω transmission line has an effective dielectric constant of 1.65. Find the shortest open-circuited length of this line that appears at its input as a capacitor of 5pF at 2.5GHz. Repeat for the inductance of 5nH.

- Solution
    - 5pF at 2.5GHz
        
        $Z_{OC}=-jZ_0cot\beta l=-j/\omega C$﻿
        
    - 5nH at 2.5GHz
        
        $Z_{OC}=-jZ_0cot\beta l=j\omega L$﻿
        

1. A 100Ω transmission line has an effective dielectric constant of 1.65. Find the shortest open-circuited length of this line that appears at its input as a capacitor of 5pF at 2.5GHz. Repeat for the inductance of 5nH.

- Solution
    
    $\begin{aligned}$
    

  

1. A 30 m long lossless transmission line with $Z_0 =50 Ω$﻿ operating at 2 MHz is terminated with a load $Z _L=(60+j40) Ω$﻿ . If the phase velocity is $v_p = 0.6c$﻿ on the line. Find:  
    a) The reflection coefficient at the load;  
    b) The standing wave ratio S;  
    c) The input impedance;  
    d) The reflection coefficient at the input  
    

- Solution
    
    a) Reflection Coefficient at the Load ($Γ_L$﻿):
    
    $⁍$
    
    b) Standing Wave Ratio (SWR):
    
    $⁍$
    
    c) Input Impedance ($Z_{in}$﻿):
    
    $Z_{in} = Z_0\frac{Z_L + jZ_0 * tan(βl)}{Z_0 + jZ_L * tan(βl)}\\$
    
    d) Reflection Coefficient at the Input ($Γ_{in}$﻿):
    
    $Γ_{in} = \frac{Z_{in} - Z_0} { Z_{in} + Z_0}=\Gamma_Le^{-2j\beta l}$
    

### Tutorial 2

![[TUT2_NetAn_1_Questions.pdf]]

![[Untitled 64.png]]

- Solution
    
    a) To be lossless: $[S]^t\cdot[S]^*=[U]$﻿
    
    b) To be reciprocal: $S_{ij}=S_{ji}$﻿
    
    c) When 2,3,4 are matched, $\Gamma = S_{11}$﻿
    
    $RL = - 20 log | \Gamma |$﻿
    
    d) When 1,3 are matched, $T=S_{42}$﻿
    
    $IL=-20log|T|$﻿
    
    e) 3 short-circuit $\to V_3=0 \to V_3^+=-V_3^-\to \Gamma_3=-1$﻿
    
    2,4 matched $\to V_2^+=V_4^+=0$﻿
    
    $[V^-]=[S][V^+]$﻿
    

![[Untitled 65.png]]

- Solution
    
    $T_l=e^{-j100\degree},\ V_4^+=T_LV_3^-, \ V_3^+=T_lV_4^+$﻿
    
    When 2 matched $V_2^+=0$﻿
    

### Exercise

![[Untitled 66.png]]

- Method 1.
    1. Convert each S matrix into its ABCD equivalent matrix.
    2. Multiply all ABCD matrices to get the overall ABCD matrix.
    3. Convert the ABCD matrix into an S matrix.
- Method 2.
    
    ![[Untitled 67.png]]
    
- Method 3.
    
    ![[Untitled 68.png]]