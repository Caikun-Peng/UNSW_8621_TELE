---
Owner: Peng, Caikun
Electives: Level 4
Last edited time: 2024-05-02
Course Progress: In Progress
Note Progress: In Progress
Note ID: PHTN4661-Tut-1
---

- Tutorial 2 Waveguides and guided modes

1. What are optical waveguides? What are optical fibres? What are their main features and applications? 

    |                 |                                                                                 |
    | --------------- | ------------------------------------------------------------------------------- |
    | **waveguide**   | A physical structure that guides electromagnetic waves in the optical spectrum. |
    | **Fibre**       | A type of waveguide that is commonly used for long-distance communication       |
    | **Feature**     | Low loss with high bandwidth                                                    |
    | **Application** | They are used in telecommunications, medical devices, and sensors               | 

2. What are optical circuits? Where and how they can be useful? What are the main issues and challenges in developing optical circuits? 
   
    |                 |                                                                                     |
    | --------------- | ----------------------------------------------------------------------------------- |
    | **Definition**  | Circuits that use light instead of electricity to perform functions                 |
    | **Application** | They can be useful in high-speed communication systems, computing, and sensing.     |
    | **Issues**      | Integration with existing electronic systems, miniaturization, and managing losses. |

3. Describe briefly how waveguide modes are defined and obtained based on wave theory. 

    > The Solution to the wave equation that satisfy the boundary conditions of waveguide, representing the possible patterns of the EM field distribution within the waveguide.

4. What are modes in general form in an optical waveguide? What are the main parameters? 

    > Modes are the distinct patterns of EM field distribution.
    > 
    > The main parameters include the mode number, propagation constant and field distribution.

5. What are TEM waves? What are TE waves? What are TM waves? 

    | Items | Describes (Lecture 2, page 23, 45)                                                                       | 
    |:-----:| -------------------------------------------------------------------------------------------------------- |
    |  TEM  | The transverse electromagnetic waves with no electric or magnetic field in the direction of propagation. |
    |  TE   | The transverse electric waves with no electric field in the direction of propagation.                    |
    |  TM   | The transverse magnetic waves with no magnetic field in the direction of propagation.                    |

6. What is a slab waveguide? How the waveguide parameters, U, W and V, are defined for a slab optical waveguide? 

    | Items   | Describes (Lecture 2, page 18)                                                                                                           | 
    | ------- | ---------------------------------------------------------------------------------------------------------------------------------------- |
    | Slab WG | The simplistic 2D waveguide. <br/>A thin film of high refractive index material sandwiched between two lower refractive index materials. |
    | U,W,V   | Defined based on the geometry and refractive indices of the waveguide.                                                                   |
    | U       | $U^2 = a^2 (k^2 n_{co}^2 - \beta^2) \quad \text{with }X=x/a$                                                                             |
    | W       | $W^2 = a^2 (\beta^2 - k^2 n_{cl}^2) \quad \text{with }X=x/a$                                                                             |
    | V       | $V^2 = U^2 + W^2 = k^2 a^2 (n_{co}^2 - n_{cl}^2) \quad \text{with }X=x/a$                                                                |

7. What is the fundamental mode of a slab waveguide? 

    > (Lecture 2, page 30) The fundamental mode of a slab waveguide is the lowest order mode, characterized by a single peak in the field distribution. 

8. What is a step-index optical fibre? What is a graded-index optical fibre 

    | Fibre types  | Definition                                                                                                   |
    | ------------ | ------------------------------------------------------------------------------------------------------------ |
    | Step-index   | The fibre has a core with a uniform refractive index surrounded by a cladding with a lower refractive index. |
    | Graded-index | The fibre has a core with a gradually changing refractive index.                                             | 

9.  How the waveguide parameters, U, W and V, are defined for a step index optical fibre? 

    > As the same as the UWV of slab waveguides but $R=r/a$

10. What is the fundamental mode of a step index optical fibre? 

    > The lowest order mode, characterized by a single peak in the field distribution, LP01

11. What is the cut-off wavelength of a step index optical fibre? 

    > The wavelength above which the fibre supports only the fundamental mode.

12. What are the main considerations in waveguide design? 

    > Including mode confinement, losses, dispersion, and compatibility with other components.

13. What is a single mode waveguide or fibre? What a multimode waveguide or fibre? Can an optical fibre be both single-mode and multimode? 

    > A single-mode waveguide is designed to support only one mode.  
    > A multimode waveguide is designed to support multiple modes.  
    > Optical fibre cannot be single mode and multimode as the same time. 

14. For a step index optical fibre with core radius $a=5\mu m$, $n_{co}=1.466$ and $n_{cl}=1.46$, what is its wavelength range of single mode operation? 

    > The wavelength is calculated by
    > $\lambda_c = \dfrac{2\pi}{V_c} a \sqrt{n_{co}^2 - n_{cl}^2}$
    > where $V_c = 2.405$ for single mode fibre.
    > Then, 
    > $\lambda_c = 1.73 \mu m$. The wavelength range is less than $\lambda_c$

15. What is ‘Gaussian Approximation’ for single-mode step index optical fibre?

    > The Gaussian Approximation is a method used to simplify the analysis of single-mode step-index optical fibres by approximating the mode field distribution with a Gaussian function.

16. For a slab waveguide
    1. Find ALL general solutions for the wave equations.

        $$
            \begin{align*}
            &\begin{aligned}
            E_y &= Ae^{-WX}            && 1<X\\
            E_y &= \left\{
                \begin{aligned}
                    & Be^{jUX} + Ce^{-jUX}\\ & \text{ or}\\
                    & (B+C)\cos{UX} + j(B−C)\sin{UX}
                \end{aligned} \right. && -1<X<1\\
            E_y &= De^{WX}             && X<-1\\&\downarrow\\
            \frac{dE_y}{dX} &= -WAe^{-WX}            && 1<X\\
            \frac{dE_y}{dX} &= −(B+C)U\sin{UX}+j(B−C)U\cos{UX} && -1<X<1\\
            \frac{dE_y}{dX} &= WDe^{WX}             && X<-1\\
            \end{aligned} \\\\
            
            &\begin{aligned}
            X & = 1 &\Rightarrow \qquad &
                \begin{aligned}
                Ae^{-W}   &= (B+C)\cos{U} + j(B−C)\sin{U}\\
                -WAe^{-W} &= −(B+C)U\sin{U}+j(B−C)U\cos{U}
                \end{aligned} \\\\
            X & = -1 &\Rightarrow \qquad &
                \begin{aligned}
                De^{-W}  &= (B+C)\cos{-U} + j(B−C)\sin{-U}\\
                WDe^{-W} &= −(B+C)U\sin{-U}+j(B−C)U\cos{-U}\\&\downarrow\\
                De^{-W}  &= (B+C)\cos{U} - j(B−C)\sin{U}\\
                WDe^{-W} &= (B+C)U\sin{U}+j(B−C)U\cos{U}
                \end{aligned}  
            \end{aligned} \\\\
            
            &\begin{aligned}
            -W((B+C)\cos{U} + j(B−C)\sin{U}) &= −(B+C)U\sin{U}+j(B−C)U\cos{U}\\
            W((B+C)\cos{U} - j(B−C)\sin{U}) &= (B+C)U\sin{U}+j(B−C)U\cos{U}\\&\downarrow\\
            
            W((B+C)\cos{U} + j(B−C)\sin{U}) &= (B+C)U\sin{U}-j(B−C)U\cos{U}\\
            W((B+C)\cos{U} - j(B−C)\sin{U}) &= (B+C)U\sin{U}+j(B−C)U\cos{U}\\&\downarrow\\
            
            W(B+C)\cos{U} + jW(B−C)\sin{U} &= (B+C)U\sin{U}-j(B−C)U\cos{U}\\
            W(B+C)\cos{U} - jW(B−C)\sin{U} &= (B+C)U\sin{U}+j(B−C)U\cos{U}\\&\downarrow\\
            
            W(B+C)\cos{U} - (B+C)U\sin{U} &= -j(B−C)U\cos{U} - jW(B−C)\sin{U}\\
            W(B+C)\cos{U} - (B+C)U\sin{U} &= +j(B−C)U\cos{U} + jW(B−C)\sin{U}\\&\downarrow\\
            
            -j(B−C)U\cos{U} - jW(B−C)\sin{U}&= +j(B−C)U\cos{U} + jW(B−C)\sin{U}\\&\downarrow\\
            
            -U\cos{U} - W\sin{U}&= +U\cos{U} + W\sin{U}\\&\downarrow\\
            
            2W\sin{U} &= -2U\cos{U}\\&\downarrow\\
            
            W &= -U\cot{U}
            \end{aligned}
            \end{align*}
        $$

    2. Find ALL possible solutions for the TE modes and give explanations.

        

17. For a slab waveguide described in 13. above, prove that its eigenvalue equation for symmetric TE modes is $W = U \tan U$. Explain what boundary conditions are used in this case.


    $$
        \begin{align*}
        &\begin{aligned}
        E_y &= Ae^{-WX}  && 1<X\\
        E_y &= B\cos{UX} && -1<X<1\\
        E_y &= De^{WX}   && X<-1\\&\downarrow\\
        \frac{dE_y}{dX} &= -WAe^{-WX}  && 1<X\\
        \frac{dE_y}{dX} &= −BU\sin{UX} && -1<X<1\\
        \frac{dE_y}{dX} &= WDe^{WX}    && X<-1\\
        \end{aligned} \\\\
        
        &\begin{aligned}
        X & = 1 &\Rightarrow \qquad &
            \begin{aligned}
            Ae^{-W}   &= B\cos{U}\\
            -WAe^{-W} &= −BU\sin{U}
            \end{aligned} \\\\
        X & = -1 &\Rightarrow \qquad &
            \begin{aligned}
            De^{-W}  &= B\cos{-U}\\
            WDe^{-W} &= −BU\sin{-U}\\&\downarrow\\
            De^{-W}  &= B\cos{U}\\
            WDe^{-W} &= BU\sin{U}
            \end{aligned}  
        \end{aligned} \\\\
        
        &\begin{aligned}
        WB\cos{U}&= BU\sin{U}\\
        WB\cos{U}&= BU\sin{U}\\&\downarrow\\
        
        W &= U\tan{U}
        \end{aligned}
        \end{align*}
    $$

19. For a slab waveguide described in 13. above, prove that its eigenvalue equation for asymmetric TE modes is $W = -U \cot U$.

    $$
        \begin{align*}
        &\begin{aligned}
        E_y &= Ae^{-WX}  && 1<X\\
        E_y &= C\sin{UX} && -1<X<1\\
        E_y &= De^{WX}   && X<-1\\&\downarrow\\
        \frac{dE_y}{dX} &= -WAe^{-WX} && 1<X\\
        \frac{dE_y}{dX} &= CU\cos{UX} && -1<X<1\\
        \frac{dE_y}{dX} &= WDe^{WX}   && X<-1\\
        \end{aligned} \\\\
        
        &\begin{aligned}
        X & = 1 &\Rightarrow \qquad &
            \begin{aligned}
            Ae^{-W}   &= C\sin{U}\\
            -WAe^{-W} &= CU\cos{UX}
            \end{aligned} \\\\
        X & = -1 &\Rightarrow \qquad &
            \begin{aligned}
            De^{-W}  &= C\sin{-U}\\
            WDe^{-W} &= CU\cos{-U}\\&\downarrow\\
            De^{-W}  &= -C\sin{U}\\
            WDe^{-W} &= CU\cos{U}
            \end{aligned}  
        \end{aligned} \\\\
        
        &\begin{aligned}
        -WC\sin{U}&= CU\cos{U}\\
        W(-C\sin{U})&= CU\cos{U}\\&\downarrow\\
        
        W &= -U\cot{U}
        \end{aligned}
        \end{align*}
    $$