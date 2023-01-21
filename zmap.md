# ZMap: Fast Internet-Wide Scanning and its Security Applications
### Zakir Durumeric (University of Michigan), et al.
### Proceedings of the 22nd USENIX Security Symposium (August 2013) ([Link](https://zmap.io/paper.pdf))

---

1. What are the paper's contributions and what did you like about the paper?  
&nbsp;&nbsp;&nbsp;&nbsp; - The paper contributes a new network scanner which is orders of magnitudes faster than the incumbents  
&nbsp;&nbsp;&nbsp;&nbsp; - ZMap has an interesting design - asynchronous, modular, extensible, SYN cookie-like overloading, custom packet and kernel bypass  
&nbsp;&nbsp;&nbsp;&nbsp; - They also ensured robust defaults by experimenting with scan rate, SYN count and diurnal variations  

2. What are questionable parts of the paper and its major limitations? (E.g., methodology issues, detail omissions, presentation problems)  
&nbsp;&nbsp;&nbsp;&nbsp; - One detail omission is that there's no follow-up study on what majorly contributes to making ZMap better than Nmap or other scanners out there - whether it is the custom packet scan methodology, or whether it is the asynchronous way of scanning, or something else  

3. What was unclear about the work, or what questions do you have?  
&nbsp;&nbsp;&nbsp;&nbsp; - One thing I didn't fully understand was how exactly the random permutation primitive root selection worked.  

4. ZMap is described as an Internet-wide scanner. However, it is not suitable for certain types of large-scale network scans that one might want to perform. What are some examples of large-scale network scans that ZMap would not be particularly suitable for?  
&nbsp;&nbsp;&nbsp;&nbsp; - ZMap inherently scans only for open ports and whether there are services listening on them. If the scan aims to understand more information like OS for example, ZMap _might not_ be able to accomplish it  
&nbsp;&nbsp;&nbsp;&nbsp; - ZMap is stateless - hence, any scan looking to understand information tied to a specific handshake, like timing scans for example, will not be accomplished by ZMap  
&nbsp;&nbsp;&nbsp;&nbsp; - ZMap is also not suitable for scans requiring multiple packets of information to be exchanged  

5. Section 4 of the paper describes various potential applications of ZMap. Describe one more potential application that is not already discussed.  
&nbsp;&nbsp;&nbsp;&nbsp; - A tangentially similar application, but one that's not discussed is to identify devices and hosts that are accidentally or unintentionally exposed to the internet  
