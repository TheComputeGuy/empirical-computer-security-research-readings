# The Spyware Used in Intimate Partner Violence
### Rahul Chatterjee (Cornell Tech), et al.
### Proceedings of the 2018 IEEE Symposium on Security and Privacy (May 2018) ([Link](https://pages.cs.wisc.edu/~chatterjee/papers/IPV_Spyware.pdf))

---

1. What are the paper's contributions and what did you like about the paper?  
&nbsp;&nbsp;&nbsp;&nbsp; - The paper studies the Intimate Partner Sureveillance (IPS) ecosystem, using an ML-enabled pipeline to identify apps that might be relevant to IPS (both single and dual-use).  
&nbsp;&nbsp;&nbsp;&nbsp; - In terms of the methodology, I liked the use of query snowballing approach to identify new and relevant search queries, similar to what a human would normally do.  
&nbsp;&nbsp;&nbsp;&nbsp; - There were also some numbing revelations like companies selling phones with in-built, jailbroken OS and tracking apps.  

2. What are questionable parts of the paper and its major limitations? (E.g., methodology issues, detail omissions, presentation problems)  
&nbsp;&nbsp;&nbsp;&nbsp; - Most of the detection engines in Fig 6 are actually anti-virus tools, rather than necessarily anti-spyware tools, most of which usually focus on desktop spyware and general malware rather than spyware apps, and Virustotal does not seem to be exactly relevant to the use-case at hand either. Thus, this section of discussion feels irrelevant to the problem at hand.  

3. What was unclear about the work, or what questions do you have?  
&nbsp;&nbsp;&nbsp;&nbsp; - The authors did not touch upon the heuristics used in the ML model for pruning false positives out of the list of apps found. This would give a good idea about what are the major factors contributing to marking an app as an IPS software, also potentially revealing gaps in analysis.  

4. Discuss at least one similarity and one difference between the IPV spyware attacks and the nation-state targeted attacks from [last Thursday's reading](https://www.usenix.org/system/files/conference/usenixsecurity14/sec14-paper-marczak.pdf).  
&nbsp;&nbsp;&nbsp;&nbsp; - In terms of similarities, both of them show classic signals of spyware - stealing location information, spying on communications, and doing all of it surreptitiously, trying to hide itself. Another similarity is that, these spyware are remotely configurable and controllable.  
&nbsp;&nbsp;&nbsp;&nbsp; - In terms of differences, one key difference in case of IPS apps is how they reach their target - in this case, physical access to the victim's device is necessary at least once, which is not the case for nation-state targeted attacks which rely on spear phishing and such techniques to lure the victims.  

5. Take any one of the proposals in Section 7 for dealing with IPV spyware, and discuss whether you think it'd be effective or not in practice.  
&nbsp;&nbsp;&nbsp;&nbsp; - OS-level protections proposed by the authors is a realistic and user-friendly way to notify the users about operations carried out by these apps. Some of the effective ways can be by showing persistent notifications when data is being exfiltrated/synced with remote servers, or a log of such attempts by different apps. Also, OS should not expose APIs to allow overriding or hiding such notifications or the log. Such measures can be implemented, making it both realistic and user-friendly.  