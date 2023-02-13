# Thou Shalt Not Depend on Me: Analysing the Use of Outdated JavaScript Libraries on the Web
### Tobias Lauinger (Northeastern University), et al.
### NDSS Symposium 2017 ([Link](https://www.ndss-symposium.org/wp-content/uploads/2017/09/ndss2017_02B-1_Lauinger_paper.pdf))

---

1. What are the paper's contributions and what did you like about the paper?  
&nbsp;&nbsp;&nbsp;&nbsp; - The paper aims to study the client-side Javascript ecosystem, and the resulting security implications.  
&nbsp;&nbsp;&nbsp;&nbsp; - I liked that the authors took a lot of effort in trying to cover as many bases as possible, including the custom AdBlock injection to flag scripts, I felt that was novel.  

2. What are questionable parts of the paper and its major limitations? (E.g., methodology issues, detail omissions, presentation problems) 
&nbsp;&nbsp;&nbsp;&nbsp; - The static analysis part could've been better, using methods like building ASTs and such, but that'd have been computationally expensive.  

3. What was unclear about the work, or what questions do you have?  
&nbsp;&nbsp;&nbsp;&nbsp; - I wonder how the situation has changed with time, whether people use more CDNs now rather than self-hosting these library scripts, or with the rise of frontend frameworks like Angular and Reac - and bundling of all scripts in one, whether it has impacted the JS ecosystem.  
&nbsp;&nbsp;&nbsp;&nbsp; - As with any vulnerability paper, even though vulnerabilities exist, doesn't mean they are necessarily exploitable in an easy manner. A good next step would be to understand how many of these _vulnerable websites_ can be actively exploited, and a framework like [expected exploitability](https://www.usenix.org/conference/usenixsecurity22/presentation/suciu) can come in really handy.  

4. What are some other potential ways (not necessarily technical) to improve the outdated JavaScript libraries situation, beyond the examples  brought up in the paper (i.e., excluding version aliasing and the ideas already stated in Section 5)? If you can't think of an example, explain whether you think the situation is hopeless.  
&nbsp;&nbsp;&nbsp;&nbsp; - One thing that stands out is that most of these vulnerable libraries are being hosted by the site itself, linked internally or inline. Similarly, a lot of injected code, i.e. via ads, analytics, etc., has a huge percentage of vulnerable JS added. In these cases, it comes down to the webmasters to keep updating the code, and that's where it is helpless to do any external mitigations.  

5. The issue highlighted in this paper is ultimately about outdated dependencies between websites and their JavaScript libraries. Describe another similar situation where one entity's security depends on another entity, and briefly discuss the similarities/differences between your situation and the paper's.  
&nbsp;&nbsp;&nbsp;&nbsp; - The packaging ecosystem, especially for Node.js, includes a lot of _transitive dependency_ patterns, where including one library as a dependency can bring in hundreds if not thousands of other dependencies. These usually go in unvetted, and a lot of these are packages by small authors or sometimes without any active maintainers. In such a case, taking over the project and injecting malicious code in the dependency isn't difficult.  
&nbsp;&nbsp;&nbsp;&nbsp; - Similar was the rush caused by the Log4shell vulnerability late last year.  
&nbsp;&nbsp;&nbsp;&nbsp; - In both these cases, a lot of software turns out to be dependent on the security of a single small piece of software.  