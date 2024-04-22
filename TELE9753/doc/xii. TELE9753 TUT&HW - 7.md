---
Owner: Peng, Caikun
Electives: Level 5
Last edited time: 2024-04-22
Course Progress: In Progress
Note Progress: Finished 
Note ID: TELE9753-TUT-7
---

# Question 
Consider a CDMA communicauon system. <br/>
1. What is the processing gain for a CDMA communication system. <br/>
2. Suppose the channel for one user is frequency selective with $h=[h_1,h_2]$. Assume that the spreading codes used for this user is $[+1,-1,-1]$, the received vector is $[r_1,r_2,r_3,r_4]$, and time-offset is one chip. Describe the steps for decoding the received vector by a Rake receiver. 

# Solution

1. The processing gain for a CDMA communication system is expressed as $W/R$, where $W$ denotes the channel bandwidth and $R$ denotes the information bandwidth.
2. Based on the information provided by the question, the first de-spreading signal is $y_1 = r_1-r_2-r_3$, and the second de-spreading signal is $y_2 = r_2-r_3-r_4$. According to $y_1$ and $y_2$, the Rake receiver decision is $\~{y} = (h_1^*y_1+h_2^*y_2) / (|h_1|^2+|h_2^2|)$. Therefore, the original transmitted signal can be determined by comparing with the constellation map Of the transmit signal.

---
[Back to note](7.%20Cellular%20System%20-%20Multiple%20Access%20and%20Interference%20Management.md)