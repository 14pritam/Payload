
### Clickjacking /UI Redress Attack
Step 1: Check for X-Frame-Options for that go to  https://securityheaders.com/

Clickjacking  is an interface-based attack in which a user is tricked into clicking on actionable content on a hidden website by clicking on some other content in a decoy website. In simple words, an attacker uses multiple transparent or opaque layers to trick a user into clicking on a button or link on another page when they were intending to click on the top level page. Thus, the attacker is “hijacking” clicks meant for their page and routing them to another page, most likely owned by another application, domain, or both.

There are three possible values for the X-Frame-Options header:
1. DENY : which prevents any domain from framing the content. The DENY setting is recommended unless a specific need has been identified for framing.
2. SAMEORIGIN : which only allows the current site to frame the content.
3. ALLOW-FROM uri : which permits the specified 'uri' to frame this page. (e.g., ALLOW-FROM http://www.example.com ).

### Example :
Website A : A website vulnerable to clickjacking which says that "You won a free iPhone!" so
that the victim gets lured by "Claiming the Prize!"
Website B: It is an attacker controlled website wherein you have the option to "Pay"
This is the exact scenario of how Clickjacking works. Attackers create an attractive website, in our case website A, to lure the victim. Create an iframe and load it in the attacker controlled domain which is website B.
In this manner the attacker manages to fool the victim and make him pay while attracting him for a free prize!
So this is how Clickjacking attack is performed.



