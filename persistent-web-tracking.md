# The Web Never Forgets: Persistent Tracking Mechanisms in the Wild
### Gunes Acar (KU Leuven), et al.
### Proceedings of the 2014 ACM SIGSAC Conference on Computer and Communications Security (November 2014) ([Link](https://securehomes.esat.kuleuven.be/~gacar/persistent/the_web_never_forgets.pdf))

---

1. What are the paper's contributions and what did you like about the paper?  
&nbsp;&nbsp;&nbsp;&nbsp; - The paper aims to study the various ways in which tracking is implemented across the web and how these methods try to defeat steps taken by privacy-conscious users. It looks at this problem from the lens of large-scale measurement and looking at prevalence across top 100,000 websites.  
&nbsp;&nbsp;&nbsp;&nbsp; - The LSO/Flash cookie concept was new to me, and the authors' approaches to detect LSO usage across browsers was interesting for me.  

2. What are questionable parts of the paper and its major limitations? (E.g., methodology issues, detail omissions, presentation problems)  
&nbsp;&nbsp;&nbsp;&nbsp; - I don't see any major limitations with the study, the authors did a good job to cover a lot of bases.  

3. What was unclear about the work, or what questions do you have?  
&nbsp;&nbsp;&nbsp;&nbsp; - I am curious to see what are the Flash cookie-like mechanisms in practice today, with the phasing out of Flash.  
&nbsp;&nbsp;&nbsp;&nbsp; - It'll also be interesting to study how today's approaches - opt-out, DNS-based blocking, uBlock-like blocking and other mechanisms are defeated by the tracking industry.  

4. For defending against persistent tracking, the paper discusses technical approaches through either disabling the tracking mechanisms, or detecting and blocking them. What are some other approaches that might help reduce persistent user tracking (including non-technical approaches)?  
&nbsp;&nbsp;&nbsp;&nbsp; - Injecting random data to pollute the tracking mechanisms is one way to tackle this problem, in an albeit adversarial way.  
&nbsp;&nbsp;&nbsp;&nbsp; - Although there's significant regulation around this space, especially with the rise of GDPR, CCPA and the like, we can see that it is still down to the tracker to honor these requests.  
&nbsp;&nbsp;&nbsp;&nbsp; - Browsers can make it harder to store and read persistent data, and enable cleaning of all avenues of data storage when the user asks to. With the largest browser today being controlled by an advertising giant, it'll be interesting to see how far things go, and proposals like FLOC do not inspire confidence.  