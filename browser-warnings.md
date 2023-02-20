# Alice in Warningland: A Large-Scale Field Study of Browser Security Warning Effectiveness
### Devdatta Akhawe (University of California, Berkeley), et al.
### Proceedings of the 22nd USENIX Security Symposium (August 2013) ([Link](https://www.usenix.org/system/files/conference/usenixsecurity13/sec13-paper_akhawe.pdf))

---

1. What are the paper's contributions and what did you like about the paper?  
&nbsp;&nbsp;&nbsp;&nbsp; - The paper aims to study the effectiveness of the security warnings served by the browser when the user visits a malware-infested website, a potential phishing website or a website that does not setup an SSL connection.  
&nbsp;&nbsp;&nbsp;&nbsp; - It uses telemetry in the browser to understand user clickthrough rate, time spent on the warning, and impact of language and extra clicks on the clickthrough rate.  
&nbsp;&nbsp;&nbsp;&nbsp; - I liked the paper's approach to understanding various aspects like warning language, time spent on various steps of the warning, dropout rate and the data collection methodologies overall.  

2. What are questionable parts of the paper and its major limitations? (E.g., methodology issues, detail omissions, presentation problems)  
&nbsp;&nbsp;&nbsp;&nbsp; - The paper mentions a low clickthrough rate for Firefox compared to Chrome, but in case of SSL errors, since Firefox allowed adding an exception, we do not have clarity on whether the clickthrough rate is correct or not. In that case, the authors could've measures the amount of times the warning was triggered but not served due to exceptions, and counted this as a click-through.  

3. What was unclear about the work, or what questions do you have?  
&nbsp;&nbsp;&nbsp;&nbsp; - It'd be interesting to know why people clicked through warnings. This can be measured in a large-scale study by serving participants randomised, optional, multiple-choice based surveys that ask them why they clicked through this warning today.  

4. Discuss some of the various factors that may impact whether a user adheres to a browser warning or not.  
&nbsp;&nbsp;&nbsp;&nbsp; - Not understanding the **significance** of the problem - If the user does not understand why a certain warning is important, they might just ignore it and go ahead with their browsing.  
&nbsp;&nbsp;&nbsp;&nbsp; - **Fatigue** - As explained in the paper, a user might just get served a lot of warnings of the same type due to misconfigurations, even due to client-side configurations. This may lead to a user ignoring *similar-looking* warnings. 
&nbsp;&nbsp;&nbsp;&nbsp; - **Confidence** about the warning being a false-positive/harmless - Sometimes, the user might feel that the problem is harmless and it won't harm to click through. For example, an SSL error on a recipe blog can be safely ignored as a risk worth taking, compared to an SSL error on a banking website.  
&nbsp;&nbsp;&nbsp;&nbsp; - **Over-confidence/curiosity** - A small percentage of users, with technical knowledge, will have either the overconfidence that the warning doesn't pose a risk, or might just be curious to see what has triggered the warning. Those users will click through.  
