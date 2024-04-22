---
Owner: Peng, Caikun
Electives: Level 5
Last edited time: 2024-04-22
Course Progress: In Progress
Note Progress: Finished
Note ID: TELE9753-TUT-6
---

# Questions
## Question 1
Consider a CDMA system with two users, which use two spreading codes $s_1 = [1, 1, 1, 1]$ and $s_2 = [1, −1, 1, −1]$ to transmit their information, respectively. Assume a flat fading channel realization of $h_1 =0.7 + 0.2j$ and $h_2 = 1.2 − 0.5j$ for the two users and a received signal vector
$$
\mathbf{r} = [0.2 + 0.7j,\ 0.8 − 0.5j,\ 0.6 − 0.3j,\ 1.3 + 0.8j] .
$$
BPSK is considered.
1. What is the processing gain of the given CDMA system?
2. How to detect the transmitted signals for the two users with Rake receiver?
3. What is the frequency diversity of the system?

## Question 2
Consider an OFDM system with total passband bandwidth $B = 1 \text{MHz}$. A single carrier system would have the symbol time $T_s = 1 = B = 1µs$. The channel has a maximum delay spread of $T_d = 5µs$, so with $T_s$ and $T_d$ there would clearly be severe ISI. Assume an OFDM system with 16-QAM modulation applied to each subchannel. To keep a small overhead, the OFDM system uses $N = 128$ subcarriers to mitigate ISI. So $T_N = N · T_s = 128µs$. The length of the cyclic prefix is set to $η = 8 > T_d = T_s$ to insure
no ISI between OFDM symbols.

For these parameters, find the subchannel bandwidth, the total transmission time associated with each OFDM symbol, the overhead of the cyclic prefix, and the data rate of the system.

## Question 3
Consider a system with total passband bandwidth $B = 1.25\text{MHz}$ and the signal travels along a path of 1.2 km. For this system, OFDM with 256 subcarriers is applied to mitigate ISI and 64-QAM modulation is applied to each subchannel.
1. If the length of the cyclic prefix is set to $η = 10$, find the subchannel bandwidth, the total transmission time associated with each OFDM symbol, the overhead of the cyclic prefix, and the data rate of the system.
2. Using the same length of the cyclic prefix as 1. but applying 128-QAM to each subchannel, what
changes will occur to the system configuration parameters obtained in 1.?

## Question 4
Consider an OFDM system. Assume that the total number of samples for DFT and IDFT is 2. The total number of subcarriers is 2 . One sample of cyclic prefix is added to each OFDM symbol. Each packet consists of one OFDM symbol for channel estimation followed by one or more OFDM symbols for data transmission. In data symbols, QPSK with $\{1 + j, −1 + j, −1 − j, 1 − j\}$ is as the modulation scheme. Suppose that the received signals are given by
$$
1.6 − 1.1j, −1.2 + 0.5j, 0.9 − 1.7j, 0.2 + 2.3j, −0.4 − 1.7j, 1.2 + 0.3j, −0.5 − 0.5j, −1.1 + 1.2j, 0.2 − 0.1j.
$$
What is estimated channel? Assuming that the estimated channel is correct, what are the transmitted signals?

## Question 5
Consider a linear equalizer with $N = 4$ and $L = 3$.
1. Express the received signals for all symbol times.
2. Identify the channel matrix $\mathbf{H}$ over all symbol times.
3. If MLSD is adopted to recover the received signals, detail the receiving process and explain why the full diversity gain is achieved.
4. If zero-forcing (decorrelating) equalizer is adopted to recover the received signals, which receive filter is used at the receiver? How does the achievable diversity gain change?


# Solution 
## Solution 1
1. The processing gain is equal to the length of the spreading code, so it is 4 for the given CDMA
system.
2. To detect transmit signals with Rake receiver, three steps are included as follows. Note that in this example, for the sake of simplicity, each user terminal receives one path, hence the MRC does not do the signal combing.
    > Step 1. De-spreading:
    > > For user 1, the despread signal is
    > > > $$
          y_1 =s_1 · \mathbf{r} = (0.2 + 0.7j) + (0.8 − 0.5j) + (0.6 − 0.3j) + (1.3 + 0.8j) = 2.9 + 0.7j
    > > > $$
    > > For user 2, the despread signal is
    > > > $$
          y_2 =s_2 · \mathbf{r} = (0.2 + 0.7j) − (0.8 − 0.5j) + (0.6 − 0.3j) − (1.3 + 0.8j) = −1.3 + 0.1j
    > > > $$
    > Step 2. Matched filtering (or MRC):
    > > For user 1, the matched filtered signal is
    > > > $$
          \~{y}_1 = \dfrac{y_1 · h_1^∗}{|h1|} = \dfrac{(2.9 + 0.7j) · (0.7 − 0.2j)}{|0.7 + 0.2j|} ≈ 4.9 + 2.8j
    > > > $$
    > > For user 2, the matched filtered signal is
    > > > $$ 
          \~{y}_2 = \dfrac{y_2 · h_2^∗}{|h1|} = \dfrac{(−1.3 + 0.1j) · (1.2 + 0.5j)}{|1.2 − 0.5j|} ≈ −1.2 − 0.4j
    > > > $$     
    > Step 3. Transmitted signal detection:
    > > For BPSK modulation, real part is a sufficient statistic for detection.<br/>
    > > For user 1, Re {ˆy1} = 4.9 > 0, the signal transmitted by user one is +1 (or information 0).<br/>
    > > For user 2, Re {ˆy2} = −1.2 < 0, the signal transmitted by user one is -1 (or information 1).
3. As the channel gains for both users have only one tap, so the frequency diversity is 1 for the system.

# Solution 2
- The subchannel bandwidth is $B_N = 1 = T_N = 7.8125 \text{KHz}$. As such, we see $B_N ≪ W_c = 1 =
2T_d = 100 \text{KHz}$, which insures negligible ISI.
- The total transmission time for each OFDM symbol is $T = T_N + ηT_s = 128 + 8 = 136µs$.
- The overhead associated with the cyclic prefix is $8/136$ which is roughly $5.88%$.
- The system transmits $log_2 16 = 4$ bits/subcarrier every $T$ seconds, so the data rate is $128 × 4/136 × 10−6 = 3.76 \text{Mbps}$. We see that this data rate is slightly less than $4B = 4 \text{MHz}$ due to the cyclic prefix overhead.

# Solution 3
1. We first calculate the symbol time of a single carrier system as $T_s = 1/B = 0.8µs$. We then calculate the delay spread as $T_d = \dfrac{1.2×103m}{3×108m/s} = 4µs$. As such, the length of the cyclic prefix $η = 10$ satisfies $η > T_d/T_s = 5$. Since $N = 256$ subcarriers are adopted, we have $T_N = NT_s = 204.8µs$. Based on these parameters, the subchannel bandwidth is $B_N = 1/T_N = 4.88 \text{KHz}$. As such, we see $B_N \ll W_c = 1/2T_d = 125 \text{KHz}$, which insures negligible ISI. The total transmission time for each OFDM symbol is $T = T_N + ηT_s = 204.8 + 10 × 0.8 = 212.8µs$. The overhead associated with the cyclic prefix is $10×0.8/212.8$ which is roughly $3.76%$. The system transmits $log_2 64 = 6$ bits/subcarrier every $T$ seconds, so the data rate is $256 × 6/212.8 × 10−6 = 7.22 \text{Mbps}$. We see that this data rate is slightly less than $6B = 7.5 \text{MHz}$ due to the cyclic prefix overhead.
2. If 128-QAM is used, then we find that the system transmits $log_2 128 = 7$ bits/subcarrier every $T$ seconds, so the data rate is $256 × 7/212.8 × 10−6 = 8.42 \text{Mbps}$.

## Solution 4
The 2-point DFT matrix is
$$ 
\mathbf{W} = \dfrac{1}{\sqrt{2}}\begin{bmatrix}1&1\\1&-1\end{bmatrix}.
$$
By removing the one CP sample, the received signals are processed as
$$
−1.2 + 0.5j, 0.9 − 1.7j, −0.4 − 1.7j, 1.2 + 0.3j, −1.1 + 1.2j, 0.2 − 0.1j,
$$
where the symbol for channel estimation is
$$
\mathbf{y} = [−1.2 + 0.5j, 0.9 − 1.7j]^T,
$$
and the two transmitted symbols are
$$
\mathbf{z}_1 = [−0.4 − 1.7j, 1.2 + 0.3j]^T,
$$
and
$$
\mathbf{z}_2 = [−1.1 + 1.2j, 0.2 − 0.1j]^T.
$$
The estimated channel is obtained as
$$
\mathbf{f} = \mathbf{Wy} = [−0.21 − 0.85j, −1.48 + 1.55j]^T.
$$
Accordingly, we obtain
$$\mathbf{f}^∗ = [−0.21 + 0.85j, −1.48 − 1.55j].
$$
The transmitted data $z_1$ is decoded by
$$
\dot{z}_1 = \mathbf{W}\mathbf{z}_1 = [0.57 − 0.99j, −1.13 − 1.41j]^T
$$
and
$$
\begin{align*}
  \ddot{z}_1 &= [(−0.21 + 0.85j)(0.57 − 0.99j), (−1.48 − 1.55j)(−1.13 − 1.41j)]^T\\
  &= [0.72 + 0.69j, −0.51 + 3.83j]^T.
\end{align*}
$$
Compare $\ddot{z}_1$ to the QPSK constellation map, the original transmitted signals are $\{1 + j, −1 + j\}$

Similarly, the transmitted data $z_2$ is decoded by
$$
\dot{z}_2 = \mathbf{W}\mathbf{z}_2 = [−0.63 + 0.78j, −0.92 + 0.92j]^T
$$
and
$$
\ddot{z}_2 = [−0.53 − 0.71j, 2.80 + 0.07j]^T.
$$
Compare \ddot{z}_2 to the QPSK constellation map, the original transmitted signals are $\{−1 − j, 1 + j\}$.

## Solution 5
1. The received signals for $N = $4 and $L = 3$ can be expressed as
    > $$
    > \begin{bmatrix}
    > y[1] \\
    > y[2] \\
    > y[3] \\
    > y[4] \\
    > y[5] \\
    > y[6]
    > \end{bmatrix}
    > =
    > \begin{bmatrix}
    > h_1 & h_2 & h_3 & 0 & 0 & 0 \\
    > 0 & h_1 & h_2 & h_3 & 0 & 0 \\
    > 0 & 0 & h_1 & h_2 & h_3 & 0 \\
    > 0 & 0 & 0 & h_1 & h_2 & h_3
    > \end{bmatrix}
    > \begin{bmatrix}
    > x[1] \\
    > x[2] \\
    > x[3] \\
    > x[4] \\
    > x[5] \\
    > x[6]
    > \end{bmatrix}
    > +
    > \begin{bmatrix}
    > w[1] \\
    > w[2] \\
    > w[3] \\
    > w[4] \\
    > w[5] \\
    > w[6]
    > \end{bmatrix}
    > .
    > $$
    As such, the received signals for time 1 to 6 are given by 
    > $$
    > \begin{equation}
    > \begin{aligned}
    > y[1] &= h_1x[1] + w[1]\\
    > y[2] &= h_2x[1] + h_1x[2] + w[2]\\
      y[3] &= h_3x[1] + h_2x[2] + h1_x[3] + w[3] \\ 
      y[4] &= h_3x[2] + h_2x[3] + h_1x[4] + w[4] \\ 
      y[5] &= h_3x[3] + h_2x[4] + h_1x[5] + w[5] \\ 
      > y[6] &= h_3x[4] + h_2x[5] + h_1x[6] + w[6]
    > \end{aligned}
    > \end{equation}
    > $$

2.  We note that Eq. (1) can be re-expressed as
    > $$
    > \begin{bmatrix}
    > y[1] \\
    > y[2] \\
    > y[3] \\
    > y[4] \\
    > y[5] \\
    > y[6]
    > \end{bmatrix}
    > =
    > \underbrace{
    > \begin{bmatrix}
    > h_1 & 0 & 0 & 0 & 0 & 0 \\
    > h_2 & h_1 & 0 & 0 & 0 & 0 \\
    > h_3 & h_2 & h_1 & 0 & 0 & 0 \\
    > 0 & h_3 & h_2 & h_1 & 0 & 0 \\
    > 0 & 0 & h_3 & h_2 & h_1 & 0 \\
    > 0 & 0 & 0 & h_3 & h_2 & h_1
    > \end{bmatrix}
    > }_{H}
    > \begin{bmatrix}
    > x[1] \\
    > x[2] \\
    > x[3] \\
    > x[4] \\
    > x[5] \\
    > x[6]
    > \end{bmatrix}
    > +
    > \begin{bmatrix}
    > w[1] \\
    > w[2] \\
    > w[3] \\
    > w[4] \\
    > w[5] \\
    > w[6]
    > \end{bmatrix}
    > .
    > $$
4. For zero-forcing equalizer, a receive filter $H^{−1}$ is used. Compared with MLSD which achieves full diversity gain, zero-forcing equalizer reduces the diversity gain to 1. For the general $M × N$ channel matrix, zero-forcing equalizer achieves the diversity gain of $M − N + 1$.

---
[Back to note](6.%20Frequency%20Diversity.md)