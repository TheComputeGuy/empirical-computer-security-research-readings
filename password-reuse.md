# The Tangled Web of Password Reuse
### Anupam Das (University of Illinois at Urbana-Champaign), et al.
### Network and Distributed System Security (NDSS) Symposium (February 2014) ([Link](https://www.cs.umd.edu/class/spring2017/cmsc818O/papers/tangled-web.pdf))

---

1. What are the paper's contributions and what did you like about the paper?  
&nbsp;&nbsp;&nbsp;&nbsp; - The paper aims to empirically study the password reuse landscape, by looking at previously leaked passwords, and non-identical password similarity for the same user across websites. 
&nbsp;&nbsp;&nbsp;&nbsp; - I liked the CDF analysis done by the authors over their dataset - they looked at different potential string modifications (4 types of string distance functions used) and did great analysis on not just reused passwords, but also passwords that were not identical. And all of this was done using off-the-shelf tools which are available to all - attacker or otherwise.  
&nbsp;&nbsp;&nbsp;&nbsp; - The appendices are very informative too, and points to a great study design.  

2. What are questionable parts of the paper and its major limitations? (E.g., methodology issues, detail omissions, presentation problems)  
&nbsp;&nbsp;&nbsp;&nbsp; - Although it is difficult in practice, the surveys conducted by the authors could've been more effective, had they been done on the users who had been observed as the subjects of multiple data breaches and similar passwords. The survey was conducted on students and professional staff at different universities, which means that it is not representative of the population, and the authors themselves mention that the responders had been exposed to password hygiene education by virtue of university intiatives. Having said that, the survey results reinforce the authors' hypothesis of poor password practices, even though the survey participants were more educated than the average internet user.  

3. What was unclear about the work, or what questions do you have?  
&nbsp;&nbsp;&nbsp;&nbsp; - 

4. The paper proposes education as a first countermeasure. How effective do you feel that user education might be?  
&nbsp;&nbsp;&nbsp;&nbsp; - I feel that password hygiene education is trite. It has been tried for years, but eventually, convenience takes precedence over security for an average user, and that will continue. If we consider password policies and password strength meters among educational measures, prior research has indicated that these also aren't always effective.  
&nbsp;&nbsp;&nbsp;&nbsp; - This potentially is because of the fatigue caused by listening to the same suggestions every time, but not having seen a huge impact by a password breach by most users out there.  

5. What are some other potential countermeasures not already discussed in the paper (e.g., beyond education, two-factor authentication, single sign-on, and coordination b/w websites)?  
&nbsp;&nbsp;&nbsp;&nbsp; - This is a problem not just about password reuse, but also about password complexity and increase in number of online services one uses with time. The paper estimated these services to be 25, and that number has definitely increased today.  
&nbsp;&nbsp;&nbsp;&nbsp; - A good password manager with an in-build password generator, that generates strong and unique passwords for each website can be a good countermeasure.  
&nbsp;&nbsp;&nbsp;&nbsp; - Although this is similar to SSO, logging into websites using identity providers (IdPs, like Google, Apple, Facebook) can also avoid people making new accounts with different passwords. The downside though, is that, a bunch of your accounts will get tied to these IdP accounts, and if your IdP account gets terminated for any reason, you might lose access to a lot of other websites.  
&nbsp;&nbsp;&nbsp;&nbsp; - Another countermeasure that can be tried is email-based authentication, wherein a code is sent to the email/other contact method as an access code, rather than having a password at all.  
&nbsp;&nbsp;&nbsp;&nbsp; - A lot of institutional single sign-ons also use public-key certificates as identification methods. Hardware tokens are also used as a second factor by a few websites, and although they are more secure and reliable, not everyone supports it.  
&nbsp;&nbsp;&nbsp;&nbsp; - Finally, standards like FIDO might be major players in shaping a passwordless future.  