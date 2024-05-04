---
Owner: Peng, Caikun
Electives: Level 5
Last edited time: 2024-05-04
Course Progress: In Progress
Note Progress: In Progress
Note ID: TELE9753-FINAL
---

# Everything you need to know about the EXAM

1) Although the topics are given here, you will need a solid grasp of other concepts as well, in particular the GSM, CDMA, OFDM, and parameters in these techniques. You will still get questions that require calculating and using some of those formulas or understanding the Rayleigh fading, the Gaussian components in the complex form, AWGN, modulations, etc.
2) The example questions below are limited. You can attempt any other questions related to the “scope of the question" for each topic, including the ones available in the homework and tutorial questions.
3) You need to revise your notes carefully, in particular the parts that cover the “scope of the question” defined below.

# Question 1
- Topic: Multiple choices and filling-in-the-blank
- Total marks: 10, including 5 sub questions: each sub question carries 2 marks
## Scope of questions:
- Key parameters or concepts in [Cellular networks](7.%20TELE9753%20Cellular%20System%20-%20Multiple%20Access%20and%20Interference%20Management.md#cellular-concept) and their relationship with system performance.
- Calculating some simple parameters via diagram
- The types/classification of technologies and their key techniques (e.g., access, modulation, coding, etc).
- Key parameters in MIMO systems. 
- Understanding the system performance (e.g., error probability, capacity, etc).
## Example questions
- All the questions that are available in the notes and the homework and tutorials.
- Frequency reuse, interference and capacity in Cellular system. What is their relationship?
- What are the multiple access technologies in GSM, CDMA or OFDM, and their corresponding advantages and disadvantages?
- How to calculate the processing gain, data rate or ship rate for different systems, such as either uplink or downlink of IS-96?
- How to calculate capacity performance for different systems, such as AWGN, slow fading, fast fading uplink or downlink?
- What advantages or benefits MIMO system can provide, and how to measure the benefits? How to get the spatial degrees of freedom given the number of transmit and receive antennas?

# Question 2
- Topic: Multi-user and opportunistic communications
- Total marks: 12, including 4 parts: each part carries 2-4 marks: 2+2+4+4=12.
## Scope of questions
- Understand the capacity region for multiple access channels, the key points of the region and how to achieve them.
- Sketch the capacity region in different conditions.
- Understanding the capacity of a slow fading channel under various schemes.
- How to maximize the data rate for each user.
- Finding the key points of a capacity region for two users given the required information such as powers and bandwidth.
## Example questions:
- All the questions that are available in the notes and the homework and tutorials.
- How to calculate capacity region for either uplink or downlink system?
- Find the method used for the capacity region and detailed steps.
- Calculation: maximize the data rate based on information obtained from questions or previous steps.

# Question 3
- Topic: Direct Sequence Spread Spectrum (DSSS) and Code Division Multiple Access (CDMA)
- Total marks: 13, including 5 parts: each part carries 1-6 marks: 2+3+1+1+6=13.
## Scope of questions
- Understanding the main stages of the system in both transmitter and receiver ends (regardless of any standards or uplink and downlink), and the advantages and disadvantages of CDMA.
- Calculating the processing gain and transmitted signal data rate based on the given parameters of the system.
- Spreading and de-spreading at a specific mobile station given the received complex signals. 
- Understanding the diversity in CDMA, such as frequency diversity.
- Understanding the near-far problems.
- Understanding how the rake receiver combines the received signals  given the paths, $h_i$(the relationship).
## Example questions
- All the questions that are available in the notes and the homework and tutorials.
- Given the received vector $[0.1-0.7j,05-0.5j,0.7-0.3j,0.3+0.8j,1.1 -0.8j, 1.5 +0.6j]$ and the spreading code $s= [1,1,-1,1, +1]$ in a BPSK scheme by a rake receiver, considering the time offset is one chip, give the output of the rake receiver by combining the signals after the de-spreading. 
- What are the near-far problem and near-far advantage? advantages and disadvantages of CDMA?
- Calculation: determine the maximum rate for two users given the transmit powers of the users as $P_1=15$,$P_2=3$ and the noise power $N_0=0.5$dB all in dB.

# Question 4
- Topic: Orthogonal frequency division multiplexing (OFDM) system
- Total marks: 15, including 5 parts: each part carries 1-4 marks: 4+4+4+2+1=15.
## Scope of questions
- Understanding the main stages of the system in both transmitter and receiver ends, the advantages of OFDM.
- Understanding how the OFDM avoids inter-symbol interference (ISI) and inter-carrier interference(ICI)
- Understanding the concept of orthogonality and the required condition for it.
- Understanding how a packet of OFDM symbols is formed at the transmitter by pilot and data symbols and how to extract the data and pilot symbols at the receiver end.
- Calculation: given enough information about the OFDM system, such as total bandwidth, number of subcarriers, modulation type, etc., you should be able to find the subchannel bandwidth, the transmission time for one OFDM symbol, the data rate of the OFDM system, and overhead of the cyclic prefix.
## Example questions
- All the questions that are available in the notes and the homework and tutorials.