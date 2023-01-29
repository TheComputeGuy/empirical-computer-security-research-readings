# Measuring Pay-per-Install: The Commoditization of Malware Distribution
### Juan Caballero (IMDEA Software Institute), et al.
### Proceedings of the 20th USENIX Security Symposium (August 2011) ([Link](https://www.usenix.org/legacy/events/sec11/tech/full_papers/Caballero.pdf))

---

1. What are the paper's contributions and what did you like about the paper?  
&nbsp;&nbsp;&nbsp;&nbsp;> The paper aims to study the Pay-per-install (PPI) ecosystem, the various actors in it, and their behaviours, to understand how malware actors have evolved in terms of distribution, while still employing anti-detection methods like packing and domain-hopping.  
&nbsp;&nbsp;&nbsp;&nbsp;> I liked the breadth of research done by the authors to study the various aspects of this ecosystem - right from understanding the usual attack chain, but also including research on how even the providers care about detection evasion, building air-tight methods of malware delivery and of course, business matters with affiliates and clients.  
&nbsp;&nbsp;&nbsp;&nbsp;> The effort put in was commendable, including manual analysis of over 300,000 binaries.  

2. What are questionable parts of the paper and its major limitations? (E.g., methodology issues, detail omissions, presentation problems)  
&nbsp;&nbsp;&nbsp;&nbsp;> 

3. What was unclear about the work, or what questions do you have?  
&nbsp;&nbsp;&nbsp;&nbsp;> One very elementary thing about this paper that I did not understand is where were the authors in the PPI chain - what did they mean by infiltration and what was the vantage point from which they were able to milk the executables (which seems like being a victim) as well as request for new executables (which sounds like something an affiliate can do).  

4. The paper discusses how PPI costs differ for hosts in different geographic regions. What might account for these price differences?  
&nbsp;&nbsp;&nbsp;&nbsp;> The aim of malware probably influences the regions that the malware authors want to operate in - certain malware which want to steal specific data, especially targetting companies, might definitely want to target high-profile businesses, especially in the west. If some malware just wants compute and machines under control, they won't necessarily need to target any specific geographic region. Some malware might rather target certain class of devices which are only sold in a specific region.  
&nbsp;&nbsp;&nbsp;&nbsp;> Given the difficulty of abuse, threat of law enforcement, difficulty of detection mechanisms and general technological awareness and cyber hygiene culture in a region, PPI costs might differ.  

5. How does the rise of PPI shift the Internet landscape for attackers or defenders? This is intentionally a very open-ended question; provide a couple examples or thoughts.  
&nbsp;&nbsp;&nbsp;&nbsp;> PPI is a significant shift in the abuse chain landscape, since it now introduces new actors in the ecosystem. Someone with access to vulnerable systems might themselves not exploit the control, but rather earn money by monetizing this control to install other spyware.  
&nbsp;&nbsp;&nbsp;&nbsp;> It also introduces a skill differential - someone good at writing malware no longer needs to worry about deploying it, and attacking systems in order to do so. They can simply pay one of the PPI providers who'll get the job done. Similarly, someone good at infiltrating systems can monetize this skill rather than spending time developing new exploits and competing with other malware authors.  
&nbsp;&nbsp;&nbsp;&nbsp;> Finally, it also poses a new challenge for cyber defenders - they now need to consider a new factor when thinking about cleaning up malware - now they have two parties to fight against, and their efforts to stop malware now need to move to higher links in the chain, like C&C takedown, etc.
