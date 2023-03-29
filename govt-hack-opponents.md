# When Governments Hack Opponents: A Look at Actors and Technology
### William R. Marczak (University of California, Berkeleyy, and The Citizen Lab), et al.
### Proceedings of the 23rd USENIX Security Symposium (August 2014) ([Link](https://www.usenix.org/system/files/conference/usenixsecurity14/sec14-paper-marczak.pdf))

---

1. What are the paper's contributions and what did you like about the paper?  
&nbsp;&nbsp;&nbsp;&nbsp; - The paper addresses the gap in research about state-led cyber operations against activists and opponents. It focuses on three things - the technology used and providers of these technologies, characterization of these attacks, and developing evidence of attacks by state and state-sponsored attacks.  
&nbsp;&nbsp;&nbsp;&nbsp; - I liked the simple, yet effective techniques used by the authors in the paper for analysis of C&C servers, as well as for getting malware samples. Particularly, using the feature of Google search that returns IP address was a smart move.  

2. What are questionable parts of the paper and its major limitations? (E.g., methodology issues, detail omissions, presentation problems)  
&nbsp;&nbsp;&nbsp;&nbsp; - I feel that as much effort that the authors have put in explaining the modus operandi and attack flows, there should've been more discussion about the empirical characterization and findings of the authors about the C2 setup and servers detected.  

3. What was unclear about the work, or what questions do you have?  
&nbsp;&nbsp;&nbsp;&nbsp; - 

4. Discuss a couple ways in which these government/nation-state attacks differ from the cybercrime attacks that we studied earlier in the semester.  
&nbsp;&nbsp;&nbsp;&nbsp; - Nation-state attacks are highly targeted, and hence, do not necessarily need to be very sophisticated in order to mask their intentions or get access to the target's system. Thus, they usually contain simple exploits like using macros or simple filename obfuscation techniques to mask the true nature of attachment.  
&nbsp;&nbsp;&nbsp;&nbsp; - These attacks are also highly social engineered, rather than technically novel. A lot of effort is put into making sure that the link or attachment is attractive enough to be clicked onto, which leads to using urgency as a tactic, or masquerading malware as security or other relevant tools. The tools used as a part of the attack chain are often off-the-shelf RATs or other spyware, rather than dedicated spyware sold only to governments.  

5. This paper doesn't get much into any defensive measures. Propose a couple defenses that might help protect the targets of government/nation-state attacks?  
&nbsp;&nbsp;&nbsp;&nbsp; - Given that the attacks used are relatively simple, it is not difficult to defeat these using well-known security practices, settings and regular software updates.  
&nbsp;&nbsp;&nbsp;&nbsp; - The simplest defensive measure against social engineering is awareness. Given that the targets are usually activists who might come in contact with many unknown, often anonymous users on the internet, it might be difficult for them to ignore emails and messages from these users. But, rather than putting blanket trust on every single user, there should be filtering and mental barriers put in place. This can include using sandboxes for downloading and executing unknown files, ignoring bait like "veryimportant.doc", etc.  
&nbsp;&nbsp;&nbsp;&nbsp; - Another, more technical solution, would be using stricter security settings (to defeat low-hanging fruit like MS Office Macros for example) in software used, even at the OS level, using more robust platforms and devices, and regularly applying security updates to the software used.  
