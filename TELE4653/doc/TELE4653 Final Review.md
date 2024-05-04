- Orthogonal  
    $$ 
        \int_{-\infty}^{\infty} f_m(t) f_n(t) dt =0,\qquad m \ne n
    $$
- Signal space
    - The dimensionality is the same as the number of the basis functions $\phi_i(t)$. 
    - To represent a waveform by a vector
        $$
            \mathbf{s}_i=\left[\int s_1(t) \phi_1(t), \int s_2(t) \phi_2(t), \cdots, \int s_i(t) \phi_i(t) \right]
        $$
- Phase State

    If $h=\dfrac{m}{p}$, then
    - For even $m$, we get $p$ different phase states
        $$\Theta_n\in\left\{0, \dfrac{\pi m}{p}, 2\dfrac{\pi m}{p}, \cdots, (p-1)\dfrac{\pi m}{p}\right\}$$
    - For odd $m$, we get $2 p$ different phase states, alternating even and odd
        $$\Theta_n \in \left\{0, \dfrac{\pi m}{p}, 2\dfrac{\pi m}{p}, \cdots, (2p-1)\dfrac{\pi m}{p} \right\}$$
- The bandwidth required for transmission of an M-ary PAM signal is
    $$W = \dfrac{R}{2\log_2 M}\text{Hz}$$
- Hamming code
    The Generate matrix
        $$G = \begin{bmatrix}
            1&1&1&0&1&0&0\\
            0&1&1&1&0&1&0\\
            1&0&1&1&0&0&1
            \end{bmatrix}=[P|I_3]$$
            $$H = [P^T|I_4]$$
            $$c = mG$$
            $$s = rH^T$$

