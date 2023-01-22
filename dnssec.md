# A Longitudinal, End-to-End View of the DNSSEC Ecosystem
### Taejoong Chung (Northeastern University), et al.
### Proceedings of the 26th USENIX Security Symposium (August 2017) ([Link](https://www.cs.umd.edu/~dml/papers/dnssec_sec17.pdf))

---

1. What are the paper's contributions and what did you like about the paper?  
&nbsp;&nbsp;&nbsp;&nbsp; - The paper aims to study the state of DNSSEC adoption at scale, also looking at whether the adoption itself is flawless and complete  
&nbsp;&nbsp;&nbsp;&nbsp; - The authors did a good job at covering width, but I specifically liked that they used VPNs for studying resolvers, an improvement over previous research, to get controlled, reproducible results  

2. What are questionable parts of the paper and its major limitations? (E.g., methodology issues, detail omissions, presentation problems)  
&nbsp;&nbsp;&nbsp;&nbsp; - The paper does not look at reasons behind low DNSSEC adoption after 20 years, that's one possible follow-up.  

3. What was unclear about the work, or what questions do you have?  
&nbsp;&nbsp;&nbsp;&nbsp; - Can DNSSEC work better if the upstream/parent zone _forces_ domain ANSes to publish/use keys. So a push rather than pull manner of doing business where the parent zone generates a key, assigns it to the child zone for the domain (potential problems being - single point of failure, what happens when domain changes the ANS provider, etc.)  

4. This paper identified numerous issues with the real-world deployment of DNSSEC. What are one or two plausible causes of these issues? How might we address them moving forward?  
&nbsp;&nbsp;&nbsp;&nbsp; - One big reason in my opinion is that DNSSEC has a lot of moving parts, and relies heavily on people to implement everything well for it to function properly end-to-end. As long as there are no incentives, this won't happen efficiently.  
&nbsp;&nbsp;&nbsp;&nbsp; - DNS record poisoning is probably not considered an enough potent threat vector by people to ensure everything works smoothly.  
&nbsp;&nbsp;&nbsp;&nbsp; - One way to address can be top-down enforcement as mentioned before, others include better incentives, standardizing and normalizing DNSSEC in practice, especially on the resolver end.
