# Before We Knew It - An Empirical Study of Zero-Day Attacks In The Real World
### Leyla Bilge and Tudor Dumitras (Symantec Research Labs)
### Proceedings of the 2012 ACM conference on Computer and Communications Security (2012) ([Link](https://users.umiacs.umd.edu/~tdumitra/papers/CCS-2012.pdf))

---

1. What are the paper's contributions and what did you like about the paper?  
&nbsp;&nbsp;&nbsp;&nbsp; - This paper aims to study zero-day attacks as they happen, by using field-gathered data, and measure statistics like duration, prevalence and characteristics of zero-day attacks.  
&nbsp;&nbsp;&nbsp;&nbsp; - The breadth of data used to understand the threat landscape was impressive, spanning various threat databases and longitudinal data as well.  
&nbsp;&nbsp;&nbsp;&nbsp; - I also liked the use of the multitude of data available with anti-virus companies, opening up many new avenues for empirical studies in the subject.  

2. What are questionable parts of the paper and its major limitations? (E.g., methodology issues, detail omissions, presentation problems)  
&nbsp;&nbsp;&nbsp;&nbsp; - One major limitation of the paper is that zero-days are usually used to target high-value targets, like major companies. This data might be missing from the dataset used by the authors.  

3. What was unclear about the work, or what questions do you have?  
&nbsp;&nbsp;&nbsp;&nbsp; - 

4. The paper identified 18 vulnerabilities seemingly exploited before disclosure over a 4 year period. Discuss whether you believe this amount is significant or not.  
&nbsp;&nbsp;&nbsp;&nbsp; - I feel, especially in today's context, that this number is very small. Given how many zero-days have been fixed in the past few months by Chrome alone, with the increase in use of software, the attack surface has definitely increased. Although, it is no wonder that zero-days have mostly been observed in Microsoft and Adobe products by the researchers, given their prevalence and use by the general populace.  
&nbsp;&nbsp;&nbsp;&nbsp; - At the same time, not just the number of vulnerabilities, but the exploitability of these are equally important. If a vulnerability is in a widely used product and is fairly easy to be exploited, then that's more valuable than a group of vulnerabilities that need to be chained and can only be exploited under certain conditions.  

5. The paper observed a significant increase in attacks using a vulnerability after disclosure. Discuss what implications this has on defending against attacks.  
&nbsp;&nbsp;&nbsp;&nbsp; - Defence after disclosure has always been a race against time. More often than not, exploits are available to bad actors before the signatures are available to the defenders, thus making it harder for AV companies.  
&nbsp;&nbsp;&nbsp;&nbsp; - Having said that, today's standards of Coordinated Vulnerability Disclosure (CVD) are a step above the Full Disclosure practices, where the vendor is given sufficient time to fix the vulnerabilities and the defenders are usually given signatures of the exploits before any public disclosure is made. That's a welcome step forward regarding disclosure.  
