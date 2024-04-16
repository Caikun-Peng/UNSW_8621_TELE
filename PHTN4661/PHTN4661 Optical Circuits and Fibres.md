---
Owner: PPeng, Caikun
tags:
  - Level-4
Last edited time: 2024-04-16
Course Progress:
  - In Progress
Notes Progress:
  - In progress
---
# Website

> [https://moodle.telt.unsw.edu.au/course/view.php?id=81753](https://moodle.telt.unsw.edu.au/course/view.php?id=81753)  

# Textbook

> https://1drv.ms/b/s!AuXfaR2IFRyojDgw_eEC7b_w0xc6?e=0mA4wV

# Instructor

|   |   |   |
|---|---|---|
|Professor|Office Room|Email|
|Gang-Ding Peng|419 EE&T|G.Peng@unsw.edu.au|

# Assessment Tasks

|   |   |
|---|---|
|Assessment Item|Weight|
|Laboratory work|25%|
|Mid-term examination|25%|
|Final examination|50%|

# Notes

## Course Overview

### Course Topics

- Overview of optical fibres and optical waveguides
- **Single mode and multimode fibres and waveguides**
- **Modal field analysis and properties**
- **Optical transmission: attenuation, dispersion and bandwidth**
- Photonic components
- Photonic circuitry and system design
- **Manufacture of optical fibre s and waveguides**
- **Optical measurement and experiment**

### Learning Outcomes

How to use the **main theoretical methods** for modelling and analysing optical waveguides and fibres

The **fundamental properties** of multi-mode and single-mode optical fibres

The main **technical issues and considerations** when using optical fibres in communication system and networks

The main **experimental methods and measurement techniques** of optical fibres

General aspects of **optical circuit and fibre design, manufacture and application**

### Fibre and waveguide related issues

- **Attenuation**
    
    Mechanisms: vibrations - UV, IR scattering
    
- **Dispersion**
    
    Phase velocity, group velocity, group index, GVD internodal, **intermodal**, **material**, polarisation
    
- Birefringence and polarisation
- **Theoretical analysis**
- **Experimental measurements**
- Fabrication and cabling

## Optical Circuits and Fibres

- Mode
    
    Multimode
    
    single-mode
- Index
    
    Step index
    
    Graded index
    
    Arbitrary index
    
- Analysis
    
    Analytical analysis
    
    Approximate analysis
    
    Numerical analysis
    

- Special designs
    
    Dispersion shifted
    
    Dispersion flattened
    
    Polarisation maintaining
    
    Twin-core / multicore
    
    Photonic crystal / bandgap
    
- **Theoretical analysis**
    
    Ray optics
    
    SI-MM, GI-MM
    
    Wave optics
    
    SI-SM, V, U, W, $\beta$﻿, $\lambda_c$﻿, $\omega$﻿
    
    Approximation methods
    
    ESI
    
    Moments
    
- **Experimental measurements**
    
    |   |   |
    |---|---|
    |$\lambda_c$|Cut-off wavelength|
    |$\omega$|Spot size|
    |$\alpha(\lambda)$|Spectral attenuation|
    |$\alpha(z)$|Fibre loss distribution|
    |$BW$|Fibre bandwidth|
    |$D(\lambda)$|Fibre dispersion|
    
- System related issues
    - **Launching and joint**
        
        Source
        
        Fibres
        
        Fibre alignment, launching / coupling, connection
        
    - **Fibre devices**
        
        Connector, coupler, grating, amplifier, isolator
        
    - System design
        
        Power-limited system consideration
        
        Bandwidth-limited system consideration
        
    - Terminal equipment
        
        Tx, Rx
        

## Basics of Optical Fibres and Waveguides

- Basics
    
    EM spectrum
    
    Optical fibre communication: $1.7\mu m-0.6\mu m$﻿
    
    Important Applications
    
    Optical communication
    
    Optical sensing
    
    Optical signal processing
    
    - Fundamental Issues in Optical Communications
        
        Signal Power
        
        Source, Attenuation, Diffraction
        
        Bandwidth
        
        Source, Dispersion, Detection
        
    - Unguided and guided source
        
        Unguided:
        
        in open air, free space
        
        sound, light, radio, microwave…
        
        Features:
        
        Good for broadcast
        
        High loss
        
        Low bandwidth
        
        Insecure
        
        Environmental influence
        
        Subject to EMI
        
        Guided
        
        in transmission medium
        
        waveguide, cable, fibre
        
        Features:
        
        Secure and reliable
        
        High bandwidth
        
        Much less environmental and EM influence
        
        Land usage
        
    
    Optical fibres
    
    Inner → Outer
    
    Core → Cladding → Coating → Strength Member → Outer Jacket
    
    $6-10\mu m$﻿ → $125\mu m$﻿ → $250\mu m$﻿
    
- Silica Optical Fibres
    
    Low loss with extremely high bandwidth
    
- Photonic Crystal Fibres
    
    Highly nonlinear
    
    Polarization maintaining
    
    Large mode area
    
    Endlessly single-mode
    
    Continuum generation
    

## Waveguide Model and Wave Method Analysis

### Maxwell Equations

$\begin{align*}$

$J$﻿: current density

$\rho$﻿: total charge density

H: magnetizing field

B: magnetic field

E: electric field

D: electric displacement field

- For optical fibres and waveguides
    
    The material is **DIELECTRIC** and **NON MAGNETIC**
    
    which means there are no free electric charges $(\rho=0)$﻿, and no electric currents $(J=0) $﻿.
    
    The Maxwell equations are simplified as
    
    $\begin{align*}$
    
      
    
    $D=\varepsilon_0 \varepsilon_rE$﻿ with $\varepsilon_r=n^2$﻿
    
    $B=\mu_0 \mu_rH$﻿ with $\mu_r=1$﻿
    
    The Light Field is $e^{- j \omega t}$﻿, the angular frequency $\omega=2\pi f = \dfrac{2 \pi c}{\lambda}$﻿. Then
    
    $\begin{aligned}$
    
      
    

### Slab Waveguides

The simplistic 2D waveguide

Infinitely along y-axis

Propagating along z-axis

The index file: $n=\left\{\begin{aligned}$﻿

Guided wave field $E(r,t)=E(x)e^{j(\beta z-\omega t)}$﻿

  

Continuity Boundary Conditions

$E_{y,1}=E_{y,2},\dfrac{dE_{y,1}}{dX}=\dfrac{dE_{y,2}}{dX}@X=\pm1$﻿

[[General Solution for Differential Equations]]

  

TE modes

Transverse Electric Field

$E_z=0$﻿

TM modes

Transverse Magnetic Field

$H_z=0$﻿

Vector wave equations

$\begin{aligned}$

Define waveguide parameters $U,W,V$﻿

$\begin{aligned}$

The scale wave equations with normalised $X=\dfrac x a$﻿

$\begin{aligned}$

The general solutions of the equations

$\begin{aligned}$

Using the boundary conditions

$\begin{aligned}$

The eigenvalue equation

$U\tan U=W$

For symmetric TE modes

$E_y=\left\{\begin{aligned}$

$\Rightarrow\qquad U\tan{U}=W$﻿

For antisymmetric TE modes

$E_y=\left\{\begin{aligned}$

$\Rightarrow\qquad U\cot{U}=-W$﻿

### Step-Index Fibre

Use the cylindrical coordinates $(r,\theta,z)$﻿ instead of $(x,y,z)$﻿

Propagating along z-axis

Symmetric waveguide

  

Electric field $E(r)$﻿ is a periodic function of $\theta$﻿

The guided wave is expressed by

$E(r,t)=E(r)e^{im\theta}e^{j\beta z}e^{-j\omega t}$

HE modes

Hybrid mode with $H_z$﻿ carrying more power than $E_z$﻿

EH modes

Hybrid mode with $E_z$﻿ carrying more power than $H_z$﻿

The wave equations with normalised $R=\dfrac r a$﻿

$\frac{\partial^2}{\partial R^2}E_z + \frac{1}{R}\frac{\partial}{\partial R}E_z + \left(U^2 - \frac{m^2}{R^2}\right)E_z = 0\\$

The solutions are expressed as the Bessel functions

$\begin{aligned}$

$J_m(UR)$﻿ is the Bessel function of the first kind of order m

$K_m(WR)$﻿ is the modified Bessel (Hankel) function of third kind of order m

  

## Waveguide Materials and Properties

- **Fundamental issues**
    
    Material requirements
    
    Attenuation
    
    Dispersion
    
    Bandwidth
    
    Strength
    
    Flexibility
    
    Material selection and waveguide design
    
    Optical loss factor in materials and fabrication
    
    Core size VS RI difference $\Delta$﻿
    
    Loss, dispersion, birefringence
    
- Waveguide materials
    
    Fused silica glass
    
    synthetic silica, the best waveguide material so far
    
    Soft glass
    
    Polymer materials
    
    Optical crystals
    
- Material properties
    - Intrinsic
        
        Material absorption
        
        Scattering
        
        Emission
        
        Nonlinear optical processes
        
        Physical and chemical
        
    - Extrinsic
        
        Impurities
        
        Scattering
        
        Bending , Stress, Environmental factors
        
        Irradiation
        
        Manufacture defects, non-uniformities
        
        Structures
        

### Fused Silica

- Key features of fused silica
    
    Very low loss
    
    Low material dispersion
    
    High mechanical strength
    
    Very low thermal expansion
    
    Very good chemical inertness
    
    Very high laser damage threshold
    
    Low dielectric constant
    
    Low dielectric loss
    
    Very high dielectric strength
    
    Good UV transparency
    
- Material Dispersion $n(\lambda)$﻿
    
    Sellmeier equation for glasses
    
    $n^2(\lambda)=1+B_1\dfrac{\lambda^2}{\lambda^2-C_1^2}+B_2\dfrac{\lambda^2}{\lambda^2-C_2^2}+B_3\dfrac{\lambda^2}{\lambda^2-C_3^2}$
    
    For fused silica
    
    $\begin{aligned}$
    
- Material Absorption $\alpha(\lambda)$﻿
    
    Electronic - optical
    
    electronic state
    
    Mechanical - IR, thermal
    
    vibrational state
    
    When the frequency of IR light matches the frequency of particular bond stretching / bending mode, the light as absorbed and the vibration or phonon is excited.
    
- **Attenuation**
    
    Fundamental Issues
    
    Material absorption
    
    UV, IR
    
    Impurities
    
    Light scattering
    
    $\Delta E=0$﻿
    
    Rayleigh scattering
    
    Mie scattering
    
    $\Delta E\ne0$﻿
    
    Raman scattering
    
    Brillouin scattering
    
    UV Absorption
    
    $\alpha_{UV}\propto\exp\left(\dfrac{hc}{\lambda E_0}\right)$﻿
    
    $h$﻿: Plank constant
    
    $c $﻿: light speed
    
    $E_0$﻿: material constant
    
    IR Absorption
    
    $\alpha_{IR}\propto\exp\left(-\dfrac{A}{\lambda}\right)$﻿
    
    A: material constant
    
    Rayleigh Scattering
    
    $\alpha_{Rayleigh}\propto\dfrac1{\lambda^4}$﻿
    
    Air bubbles
    
    Impurity
    
    Wrong bond
    
    Structure inhomogeneity
    
    Core-cladding interface
    
    Impurity Absorption
    
    Water (-OH bond) in silica has fundamental resonant absorption at wavelength at $2.72$﻿$\mu m$﻿.
    
    This resonance has overtone absorption peaks scattered across the optical communication windows.
    
    ![[Untitled 5.png|Untitled 5.png]]
    
    - Attenuation or Loss Coefficient $\alpha$﻿
        
        dB per unit length (dB/cm, dB/m, dB/km)
        
        $\mathbf{P(z)} = \mathbf{P_0} 10 ^{-\dfrac{\alpha}{10}\mathbf{z}}\\$
        
        1 per unit length (1/cm, 1/m, 1/km)
        
        $\mathbf{P(z)=P_0}e^{-\alpha\mathbf{z}}\\$
        
          
        
        Neper per unit length
        
        $\mathbf{P(z)=P_0}e^{-\alpha\mathbf{z}}\\$
        
- Bending related properties
    
    - Key issues
        
        Bending loss
        
        Mode coupling
        
        Applications
        
        Waveguide design
        
        Measurement
        
        Sensing
        
        Tapping optical signal
        
    
    Two kinds of Bending
    
    - Micro-bending
        
        Random core deformation
        
        Size fluctuation
        
        Statistical parameters
        
        RMS deviation, correlation length
        
        ![[Untitled 1 3.png|Untitled 1 3.png]]
        
    
    - Macro-bending
        
        Bends
        
        Curves
        
        Radius of curvature: R
        
        ![[Untitled 2 3.png|Untitled 2 3.png]]
        
    
    All bending introduce radiation loss as well as mode coupling or mixing
    
    |   |   |
    |---|---|
    |Radiation loss|Bending effect on mode field|
    |Mode coupling|core to cladding mode coupling|
    |Cladding mode loss|absorption at the interface|
    
    Radiation loss due to macro-bending
    
    $\alpha_R(\lambda)=c_1(\lambda)e^{-c_2(\lambda)R}$﻿
    
    For MM fibre, the critical radius
    
    $R_{c,MM}=\dfrac{2n^2_{co}\lambda}{4\pi NA^3}$﻿
    
    For SM fibre, the critical radius
    
    $R_{c,SM}=\dfrac{20\lambda}{NA^3}\left( 2.748-0.996 \dfrac{\lambda}{\lambda_c} \right)^{-3}$﻿
    
      
    

## Waveguide Coupling and Light launching

## Light Launching

The initial field distribution $E_0(x,y)$﻿ at the input end of the waveguide

$E_0(x,y)=\underbrace{\displaystyle\sum_{i=1}^{N}{A_iE_i(x,y)}}_{\text{Guided modal field}}$﻿

$E_0(x,y)$﻿ is decomposed into a linear combination of the guided modal fields and unguided modal fields (_leaky modes_)

The unguided fields may be guided in the cladding, as cladding mode

Cladding mode is particularly detrimental to accuracy in fibre measurement and must be removed effectively by

$n_{coating}>n_{cladding}$﻿

The launching efficiency, $\eta$﻿, of the guided mode

$\eta=\dfrac{\left|\displaystyle\int_0^{\infty}{\vec{E_0}\cdot\vec{E_i}ds}\right|^2}{\displaystyle\int_0^{\infty}{|E_0|^2ds}\displaystyle\int_0^{\infty}{|E_i|^2ds}}=(\text{overlap integral of fields})^2$﻿

- Gaussian Approximation
    
    The fundamental mode field of a SI fibre
    
    $E_z(R)=\left\{\begin{aligned}$﻿
    
    The fundamental mode field can be approximately represented by  
    Gaussian function (  
    **Gaussian Approximation**)
    
    $E_z(r)=e^{-{r^2}/{2\omega^2}}$﻿
    
    Where the parameter, $\omega$﻿, is called **Spot Size**
    
- Spot Size
    
    Definition
    
    The radial distance from the fibre axis to the position where the electric field amplitude of light drops to $1/e$﻿ (37%) of the maximum value at the centre of the fibre core.
    
    $E(\omega)=\dfrac{1}{e}E_{max}$﻿
    
    For SI fibre
    
    $\dfrac{\omega}{a}=0.65+\dfrac{1.62}{V^{3/2}}+\dfrac{2.88}{V^6}$﻿
    
- Source to fibre light launching
    - Issues
        
        Source and fibre related issues
        
        |   |   |
        |---|---|
        |LED|Power, wavelength, radiation area, pattern|
        |LD (Laser Diode)|Power, wavelength, spot size|
        |MM|Core diameter, index profile, NA|
        |SM|Spot size|
        
        Technical issues
        
        Tilt, offset. Separation
        
        When launching light into optical fibres we need to maximize the efficiency
        
        Select source that match the fibre to be used
        
        LED → MM, LD → SM
        
    - Source to MM fibres
        1. Launching efficiency of a source to an SI-MM fibre
            
            $\eta=\underbrace{\vphantom{\left\{\begin{aligned}$﻿
            
            $\sigma$﻿ is the directivity factor of the source: $I(\theta)=I_0\cos^{\sigma}\theta$﻿
            
            For LED, $\sigma\sim1$﻿. For LD, $\sigma\sim20$﻿.
            
        2. Launching efficiency of a Lambertian source to a GI-MM fibre
            
            For a GI-MM fibre
            
            $n^2(r)=n_1^2\left[1-2\Delta\left(\dfrac{r}{a}\right)^a\right]$﻿
            
            the launching efficiency is
            
            $\eta = \left\{\begin{aligned}$﻿
            
        3. Launching efficiency of a source to a GI-MM fibre
            
            For a GI-MM fibre,
            
            $n^2(r)=n_1^2\left[1-2\Delta\left(\dfrac{r}{a}\right)^a\right]$﻿
            
            and a source of intensity radiation pattern
            
            $I(\theta)=I_0\cos(l\theta)$﻿
            
            the launching efficiency $\eta$﻿ between the light source and the fibre is
            
            $\eta=\dfrac{2}{b^2}\displaystyle\int_{0}^{a'}{rdr}\left\{1-\left[\left(1-2\Delta n_1^2\right)+2\Delta n_1^2\left(\dfrac{r}{a}\right)^\alpha\right]^{\frac{l+2}{2}}\right\}$﻿
            
            $b$﻿ is the radius of emitting area of source
            
            $a'=\min(a,b)$﻿
            
    - Source to SM fibres
        
        Consideration
        
        SM fibre → Fundamental mode only → Gaussian field description → Spot size $\omega $﻿ given by V
        
        Launching efficiency of a LD source to an SI-MM fibre
        
        $\eta = \left( \dfrac{2 \omega_1 \omega_2}{\omega_1^2 + \omega_2^2} \right)^2$﻿
        
        the spot size of SI-SM fibre
        
        $\dfrac{\omega}{a} = 0.65 + \dfrac{1.62}{V^{3/2}} + \dfrac{2.88}{V^6},\ 1.2 \le V \le 4 \text{ for fundamental mode only}$﻿
        

### Waveguide Connection

- Key Issues
    
    Different for MM and SM cases
    
    Fibre related issues
    
    |   |   |
    |---|---|
    |MM to MM|Core diameter, index profile, NA, direction|
    |SM to SM|Spot size|
    
    Technique related issues
    
    |   |   |
    |---|---|
    |Offset|Lateral misalignment of fibre cores|
    |Tilt|Angular misalignment of fibre cores|
    |Separation|Gap between fibre ends|
    |Distortion||
    |Fibre end|Finish and Fresnel reflections|
    
- MM to MM Fibre Connection
    
    - Joint loss
        1. Joint Loss due to **NA mismatch** of MM fibres
            
            $L_{NA}=\left\{\begin{aligned}$﻿
            
            $NA_1:$﻿ input Numerical Apertures
            
            $NA_2:$﻿ output Numerical Apertures
            
        2. Joint Loss due to **core mismatch** of MM fibres
            
            $L_{a}=\left\{\begin{aligned}$﻿
            
            $a_1:$﻿ input core radii
            
            $a_2:$﻿ output core radii
            
        3. Joint Loss due to **Fresnel reflection** of MM fibres
            
            $L_n=-10\log\left(1-\left(\dfrac{n_1-n_2}{n_1+n_2}\right)^2\right)$﻿
            
            $n_1:$﻿ input core refractive index
            
            $n_2:$﻿ output core refractive index
            
        4. Joint Loss due to **index mismatch** of GI-MM fibres
            
            For GI-MM fibre $n^2(r)=n_1^2\left[ 1 - 2 \Delta \left( \dfrac{r}{a} \right)^\alpha \right]$﻿
            
            $L_\alpha=\left\{\begin{aligned}$﻿
            
            $\alpha:$﻿ the index profile parameter
            
    
    - Power Loss
        
        1. Power Loss with offset
            
            $L_d=-10\log\left( 1-\dfrac{d}{2a}\right)$﻿
            
            $a:$﻿ radius of fibre core
            
        2. Power Loss with tilt
            
            $L_\theta=-10\log\left( 1-\dfrac{\theta}{2\theta_{C,L}}\right)$﻿
            
            $\theta_{C,L}:$﻿ critical launching angle of fibre
            
        3. Power Loss with separation
            
            $L_D=-10\log\left( 1 - \dfrac{a}{a+D\tan\theta_{C,L}}\right)^2$﻿
            
            $D:$﻿ separation between two fibres
            
        
          
        
        Offset
        
        ![[Untitled 3 2.png|Untitled 3 2.png]]
        
        Tilt
        
        ![[Untitled 4 2.png|Untitled 4 2.png]]
        
        Separation
        
        ![[Untitled 5 2.png|Untitled 5 2.png]]
        
    
- SM to SM Fibre Connection
    1. Power transmission between two SM fibres
        
        $T=\dfrac{\left|\displaystyle\int_0^{\infty}G_1 G_2 r dr\right|^2}{\displaystyle\int_0^{\infty}|G_1|^2 r dr \displaystyle\int_0^{\infty}|G_2|^2 r dr}=(\text{overlap integral of fields})^2$﻿
        
        Fibre connection loss of SM fibre is only **Spot size mismatch**
        
    2. Power Transmission with **spot size mismatch**
        
        $T_\omega=\left(\dfrac{2 \omega_1 \omega_2}{\omega_1^2 + \omega_2^2}\right)^2$﻿
        
    3. Power Transmission with **offset**
        
        $T_d=\left(\dfrac{2 \omega_1 \omega_2}{\omega_1^2 + \omega_2^2}\right)^2\exp\left[-\dfrac{2d^2}{\omega_1^2 + \omega_2^2}\right]$﻿
        
    4. Power Transmission with **tilt**
        
        $T_\theta=\left(\dfrac{2 \omega_1 \omega_2}{\omega_1^2 + \omega_2^2}\right)^2\exp\left[-\dfrac{2(\pi n_2 \omega_1 \omega_2 \theta)^2}{(\omega_1^2 + \omega_2^2)\lambda^2}\right]$﻿
        
    5. Power Transmission with **separation**
        
        $T_{D,\omega} = \dfrac{4\left[ 4Z^2 + \dfrac{\omega_1^2}{\omega_2^2}\right]^2}{\left[ 4Z^2 + \dfrac{\omega_1^2 + \omega_2^2}{\omega_2^2} \right]^2 + 4Z^2 \dfrac{\omega_2^2}{\omega_1^2}} \quad \text{with} \quad Z = \frac{D}{n_2 k_1 \omega_1 \omega_2}$﻿
        
    6. Power Transmission with **offset**, **tilt** and **separation**
        
        $\begin{aligned}$﻿
        
        The same formular may be used to work out the launching efficiency between a laser source and a SM fibre
        

## Dispersion and Bandwidth

### Phase Velocity, Group Velocity and GVD

Assume a practical modal field that may be expressed approximately as

$\omega_1=\omega$﻿ and $\omega_2 = \omega + d\omega$﻿

Correspondingly the propagation constants are

$\beta_1= \beta$﻿ and $\beta_2 = \beta + d\beta$﻿

The electric field along a fibre

$\begin{aligned}$﻿

The Group velocity: speed of moving wavelet

$V_g=\dfrac{d\omega}{d\beta}$﻿

The Phase velocity: speed of moving phase

$V_p=\dfrac{\omega}{\beta}$﻿

- Important parameters
    
    **Group delay** or **time delay,** **$\tau$**﻿**,** over length $L$﻿
    
    $\tau = \dfrac{L}{V_g}\qquad[s]$﻿
    
    **Group delay,** **$\bar\tau$**﻿**,** per unit length
    
    $\bar{\tau} \equiv \dfrac{\tau}{L}\qquad[s/m]$﻿
    
    **Group Velocity Dispersion (GVD)** per unit angular frequency
    
    $\text{GVD} \equiv \dfrac{d\bar{\tau}}{d\omega} \qquad [s^2/m]$﻿
    
    GVD, D, per unit wavelength
    
    $D \equiv \dfrac{d\bar\tau}{d\lambda}\qquad[s/m^2]$﻿
    
    $\omega = \dfrac{2 \pi c}{\lambda} \to d\omega = -\dfrac{2 \pi c}{\lambda^2} d\lambda \to \tau = \dfrac{L}{V_g} = -L \dfrac{\lambda^2}{2 \pi c} \dfrac{d\beta}{d\lambda}$﻿
    
    In a uniform medium
    
    $\beta = n(\lambda)\dfrac{2 \pi}{\lambda} \to $﻿
    
    $V_p = \dfrac{\omega}{\beta}=\dfrac{c}{n}$﻿, $V_g = \dfrac{d\omega}{d\beta}=\dfrac{c}{n_g},\qquad n_g=n-\lambda\dfrac{dn}{d\lambda}=\text{Group index}$﻿
    
    Hence,
    
    $\tau(\lambda)=\dfrac{L}{V_g}=L\dfrac{d\beta}{d\omega}=\dfrac{L}{c}\left(n-\lambda\dfrac{dn}{d\lambda}\right)$﻿
    
    $\dfrac{d\tau}{d\lambda}=-\dfrac{L}{c}\lambda\dfrac{d^2n}{d\lambda^2}$﻿
    

### Material Dispersion

The pulse broadening $\Delta\tau$﻿ of an optical impulse with a wavelength width $\Delta\lambda$﻿ can be found as

$\Delta\tau=\dfrac{d\tau}{d\lambda}\Delta\lambda=-\dfrac{L}{c}\lambda\dfrac{d^2n}{d\lambda^2}\Delta\lambda$﻿

Define a material dispersion parameter $D $﻿ as

$D=-\dfrac{\lambda}{c}\dfrac{d^2n}{d\lambda^2}\qquad[ps/nm\cdot km]$﻿

With known D, the pulse broadening

$\Delta\tau=DL\Delta\lambda$﻿

Normally $\sigma_m = \Delta\tau$﻿ and $S_\lambda= \Delta\lambda$﻿. Hence the pulse broadening due to material dispersion, $\sigma_m$﻿

$\sigma_m = DLS_\lambda$﻿

For an SI fibre, the normalised propagation constant, $b$﻿

$b = \dfrac{\beta^2 - k_2^2}{k_1^2 - k_2^2} = \dfrac{W^2}{V^2}\qquad\text{with }k_1=\dfrac{2 \pi n_1}{\lambda},\ k_2=\dfrac{2 \pi n_2}{\lambda}\text{ and }W=1.1428V-0.996$﻿

$\to \Delta\tau=-\dfrac{L}{2 \pi c}\Delta\lambda\dfrac{d\lambda}{d}\left(\lambda^2\dfrac{d\beta}{d\lambda}\right),\qquad \sigma_m=-\dfrac{S_\lambda L}{c}\dfrac{n^2 \Delta}{\lambda}V\dfrac{d^2Vb}{dV^2}\approx-\dfrac{S_\lambda L}{c}\dfrac{n^2 \Delta}{\lambda}V\dfrac{2}{V^2}$﻿

### Impulse Response

The impulse response of a step-index multimode optical fibre can be derived by this integral:

$h(t)=\displaystyle\int_{0}^{\theta_c}{\delta(t-\tau(\theta))I(\theta)\sin\theta d\theta}$﻿

Where $I(\theta)$﻿ is the radiation pattern of optical source

The average time delay $\tau_{av}$﻿

$\tau_{av}=\dfrac{\displaystyle\int_{-\infty}^{\infty}th(t)dt}{\displaystyle\int_{-\infty}^{\infty}h(t)dt}$﻿

The RMS pulse width $\sigma$﻿

$\sigma^2=\dfrac{\displaystyle\int_{-\infty}^{\infty}(t-\tau_{av})^2h(t)dt}{\displaystyle\int_{-\infty}^{\infty}h(t)dt}$﻿

Pulse Broadening

$\sigma=\sqrt{\sigma_{in}^2 + \sigma_{int}^2 + (\sigma_m + \sigma_w)^2}$﻿

Bandwidth

$B=\dfrac{0.25}{\sigma}$﻿

# Tutorials

[[Tutorials reference answers]]