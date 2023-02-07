# Trafficking Fraudulent Accounts: The Role of the Underground Market in Twitter Spam and Abuse
### Kurt Thomas (University of California, Berkeley), et al.
### Proceedings of the 22nd USENIX Security Symposium (August 2013) ([Link](https://www.inwyrd.com/blog/wp-content/uploads/2010/03/usenix20131.pdf))

---

1. What are the paper's contributions and what did you like about the paper?  
&nbsp;&nbsp;&nbsp;&nbsp; - The paper aims to study the fraudulent account sale ecosystem, the monetary side of it, as well as how these sellers evade detection and automated barriers.  
&nbsp;&nbsp;&nbsp;&nbsp; - I liked that the paper focused on getting good sources of data, directly from Twitter. They used a wide variety of signals like time taken to fill the form, user agents used, activities post account creation, etc., which are very effective features that can help them reduce false positives and reinforce classification. At the same time, it also brings into perspective, the amount and granularity of information these big platforms collect.  
&nbsp;&nbsp;&nbsp;&nbsp; - I also liked that the paper found a few ways to identify resellers vs account creators.  

2. What are questionable parts of the paper and its major limitations? (E.g., methodology issues, detail omissions, presentation problems)  
&nbsp;&nbsp;&nbsp;&nbsp; - One thing I feel can be problematic is that the authors used patterns generated based on email ID to corroborate with patterns generated based on usernames to identify/cluster the merchants. But given that a lot of these email IDs will be bought by the merchant themselves, the email IDs might not necessarily follow any specific naming pattern (an example pattern can be {CamelCaseWords}{5 numbers}@provider.tld. Now, it is not necessary that all the email IDs used by the merchant follow the exact same pattern, making it a potentially unreliable indicator)  

3. What was unclear about the work, or what questions do you have?  
&nbsp;&nbsp;&nbsp;&nbsp; - The significance of the account naming pattern feature generation (using common character classes) was not clear to me.  

4. Compare and contrast the abuse vector and underground ecosystem in this paper with those of the previous papers we've read. Provide a few similarities and differences.  
&nbsp;&nbsp;&nbsp;&nbsp; - This paper looks at the economies of sale of accounts, primarily Twitter, but also touching upon the sale of email accounts tangentially a few times. While this seems like a one-person business, a lot of the process is, like other papers, externalized.  
&nbsp;&nbsp;&nbsp;&nbsp; - This paper also uses good amount of data to build their heuristics, and this makes it unique from a defender's perspective, compared to the other papers we saw. They are able to generate a good quality pipeline and model because of both the unique nature of abuse here, as well as the less-fragmented nature of the ecosystem.  
&nbsp;&nbsp;&nbsp;&nbsp; - As said earlier, though there are certain parts of the process externalized, this is a largely solo venture. This makes it easier to pinpoint the actors and take swift takedown actions.  
