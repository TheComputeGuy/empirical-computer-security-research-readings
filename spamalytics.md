# Spamalytics: An Empirical Analysis of Spam Marketing Conversion
### Chris Kanich (University of California, San Diego), et al.
### Proceedings of the 15th ACM conference on Computer and Communications Security (October 2008) ([Link](https://www1.icsi.berkeley.edu/pubs/networking/2008-ccs-spamalytics.pdf))

---

1. What are the paper's contributions and what did you like about the paper?  
&nbsp;&nbsp;&nbsp;&nbsp;> The paper aims to study the spam economy, but from the perspective of a scammer, looking at aspects like conversion rate and how it affects earnings.  
&nbsp;&nbsp;&nbsp;&nbsp;> The paper touches on a lot of interesting tangents of the spam ecosystem, not just monetary, but also in terms of the infrastructure and technical complexity, impacts of blacklists and anti-spam measures, etc.  
&nbsp;&nbsp;&nbsp;&nbsp;> Just as an aside, I liked how the paper linked tables, figures and references as in-document hyperlinks whenever they were mentioned. It made it easier to go and look at them without manually searching for the table in the paper.  

2. What are questionable parts of the paper and its major limitations? (E.g., methodology issues, detail omissions, presentation problems)  
&nbsp;&nbsp;&nbsp;&nbsp;> The paper does not mention anything about how the infiltration took place and how they were able to inject their own proxies into the Storm network.  

3. What was unclear about the work, or what questions do you have?  
&nbsp;&nbsp;&nbsp;&nbsp;> I am not clear about how the worker nodes generated delivery reports.  

4. As highlighted by this paper, spam is an economic proposition. Discuss a couple examples (potentially going beyond this paper) of how this financial motivation influences how spam campaigns are run.  
&nbsp;&nbsp;&nbsp;&nbsp;> The first and foremost element of spam is that a spam campaign, especially email spam is easy to set up, easy and cheap to run, and being unsolicited, difficult to stop, almost a whack-a-mole scenario.  
&nbsp;&nbsp;&nbsp;&nbsp;> In such a case, spammers can focus on spending money on bullet-proofing their campaigns rather than focusing on delivery. They can spend money on building more resilient technology, building multiple fronts for serving spam/malicious content and jumping hosts and domains when blacklisted.  
&nbsp;&nbsp;&nbsp;&nbsp;> Papers like [PharmaLeaks](https://cseweb.ucsd.edu/~apitsill/papers/UsenixSec12.pdf) talk about other aspects of the spam ecosystem, like affiliates, advertisement networks and the customers themselves.  

5. Provide your thoughts on the ethics and/or legality of the methodology used in this paper (Section 4). Do you have any concerns, or do you think the methodology is fine, as argued in Section 4.5?  
&nbsp;&nbsp;&nbsp;&nbsp;> While one can always argue that by having control of the proxies, the authors could've used that power to not send spam rather than sending unsolicited emails, I feel that the methodology was airtight. They took care to ensure that they didn't send any spam on their own, while also ensuring that users that interacted with these websites were shielded from malware and abuse.  
&nbsp;&nbsp;&nbsp;&nbsp;> In my opinion, this is like a bitter pill that researchers had to take, because to conduct research using that position in the chain, they'd have to become an active member of the abuse chain to get meaningful insights about their behaviour. The ethics of this is tangentially similar to what spies and such intelligence gathering have to do while investigating threats in real life.  
