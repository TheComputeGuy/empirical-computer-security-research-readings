# Comprehensive Experimental Analyses of Automotive Attack Surfaces
### Stephen Checkoway (University of California, San Diego), et al.
### Proceedings of the 26th USENIX Security Symposium (August 2017) ([Link](https://www.cs.umd.edu/~dml/papers/dnssec_sec17.pdf))

---

1. What are the paper's contributions and what did you like about the paper?  
&nbsp;&nbsp;&nbsp;&nbsp; - The paper studies the automobile security ecosystem from the lens of remote compromise - by studying the possible attack vectors, exploitable vulnerabilities that do not need direct physical access, and ways of remote exploitation.  
&nbsp;&nbsp;&nbsp;&nbsp; - I liked the tone and structure of the paper - having enough technical details but with sufficient depth too - not too shallow, not too deep.  

2. What are questionable parts of the paper and its major limitations? (E.g., methodology issues, detail omissions, presentation problems)  
&nbsp;&nbsp;&nbsp;&nbsp; - Quite a few of the vulnerabilities mentioned in the document are highlighted as not to be "direct physical access" but either need communication in close range or exploitation of some other systems for establishing access, not all scenarios of which are plausible.  

3. What was unclear about the work, or what questions do you have?  
&nbsp;&nbsp;&nbsp;&nbsp; - 

4. Based on the car systems/components evaluated and the threat models/attack vectors considered in this paper, discuss the extent to which you think the paper's observations/conclusions about modern car vulnerabilities generalize to the modern car ecosystem broadly. For example, do you think all modern cars are similarly affected, certain types of cars are more/less affected, etc.?  
&nbsp;&nbsp;&nbsp;&nbsp; - I feel that the industry has moved forward in the past ten years, although some of the gaps still remain. The paper discusses various attack vectors, some of which are vulnerable by design and cannot be mitigated by software updates.  
&nbsp;&nbsp;&nbsp;&nbsp; - With time, automotive security standards have improved and most of today's vehicles no longer use unencrypted communication or unsigned updates and communications. But, with software increasingly driving cars today and as connectivity increases, it has led to kicking the can down the road. Problems are now seen more deeper down the system, with multiple vulnerabilities needing to be chained.  
&nbsp;&nbsp;&nbsp;&nbsp; - Some classic examples of this are the "turn-key-to-start" issue in Hyundai and Kia cars earlier this year, or the [CAN Injection](https://kentindell.github.io/2023/04/03/can-injection/) attacks popularized recently.  
&nbsp;&nbsp;&nbsp;&nbsp; - All-in-all, with increasing influence of software and connectivity in modern cars, the attack surface has definitely increased, and the onus is on companies to build secure systems, although historically, they've not done a great job at it.  

5. The paper proposes several recommendations for addressing these modern car vulnerabilities. Choose one and discuss how effective you think this recommendation would be in practice. (This can include factoring in how feasible/likely it is for stakeholders to adopt the recommendation in practice, as well as how effective the recommendation could be if adopted.)  
&nbsp;&nbsp;&nbsp;&nbsp; - A lot of the recommendations in the paper pertain to hardening the software vulnerabilities, and taking all of these steps together, can be very effective in hardening the system overall.  
&nbsp;&nbsp;&nbsp;&nbsp; - Steps like using a firewall with whitelist for outbound connections, keeping the device OS light by removing unnecessary services (like telnet for example), ASLR and use of memory-safe code APIs, etc. are steps that can be very easily implemented, along with using strong root passwords and strong defaults. Although this might not necessarily remove all vulnerabilities, it definitely slows the attacker down and strengthens the security of the system overall.  
