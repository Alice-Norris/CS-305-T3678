# CS-305-T3678

Briefly summarize your client, Artemis Financial, and their software requirements. Who was the client? What issue did they want you to address?
The client, Artemis Financial, is a financial firm, managing the financial interests of their clients, including retirement plans, insurance, investments, etc.
Artemis Financial wanted to update their software, creating a web application using a RESTful interface to securely transmit, store, and manage data for their clients.

What did you do particularly well in identifying their software security vulnerabilities? Why is it important to code securely? What value does software security add to a company’s overall wellbeing?
Security is of utmost impoertance in an age where data is increasingly stored away from and physically out of the hands of the people it is pertinent to. Since this data must be transmitted across global networks, any compromise or weakness of security can have devastating impacts on the owner(s) of the data. A company with less than appropriate software security can be held financially responsible for damages caused by insufficient security. Lives, property, and reputations can be damaged by insufficient security. When identifying vulnerabilities, I feel that I addressed dependencies the best, making sure to use static analysis tools to catch and mitigate as many vulnerabilities introduced by external code as possible, since external code is basically equivalent to untrusted data.

What about the process of working through the vulnerability assessment did you find challenging or helpful?
Ensuring that the cryptographic ciphers and protocols used was perhaps the most challenging, and absolutely the most vital. Once data is sent, it cannot be unsent, and any transmission must be as secure as possible. 

How did you approach the need to increase layers of security? What techniques or strategies would you use in the future to assess vulnerabilities and determine mitigation techniques?
I attempted to approach increasing security incrementally, taking each piece of the code seriously and ensuring that any vulnerabilities I was aware of were mitigated to the best of my ability. In the future, I would like to be more well-versed in what strategies are commmonly used to attempt to circumvent security.

How did you ensure the code and software application were functional and secure? After refactoring code, how did you check to see whether you introduced new vulnerabilities?
What resources, tools, or coding practices did you employ that you might find helpful in future assignments or tasks?
When adding new dependencies, I ran the dependency check as each was added, in an attempt to prevent vulnerabilities from becoming "baked in" to the code, becoming too far entrenched to easily remove. Where possible, I tried to keep the code that I added as close to the documentation as possible, as forcing things to work with work-arounds can drastically increase vulnerability. I used dependency checks, the vulnerability databases online, and the maven dependency tree and build tools to streamline dependencies as much as possible, mitigate vulnerabilities that could not be removed as best I could, and updated new dependencies as much as possible while still maintaining compatibility with Java SE 8.

Employers sometimes ask for examples of work that you have successfully completed to demonstrate your skills, knowledge, and experience. What from this particular assignment might you want to showcase to a future employer?
I'd definitely want to show an employer my configuration files for the Spring framework, my security configuration class, and the work I did with the Maven build tool. 
