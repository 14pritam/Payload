### DMARC
DMARC also known as Domain-based Message Authentication Reporting and Conformance is a free and open technical specification that is used to authenticate an email by aligning 
SPF and DKIM mechanisms. By having DMARC in place, domain owners large and small can fight business email compromise, phishing and spoofing.

### What are the Benefits of DMARC Record?

The main benefits of DMARC Record could be listed as followed:

1.Reputation: Publishing a DMARC record protects your brand by preventing unauthenticated parties from sending mail from your domain.

2.Visibility: DMARC reports increase visibility into your email traffic by letting you know who is sending email from your domain.

3.Security: DMARC helps the email community establish a consistent policy for dealing with messages that fail to authenticate. This helps the email ecosystem as a whole become
more secure and more trustworthy.

### To find DMARC Record of the domain use online tool https://mxtoolbox.com/ to read the records.

Case-I:

Here as you can see there is the line “Your email service provider is Google Apps”, hence it is an email domain, but here both the statements “DMARC Policy Not Enabled” and 
“DMARC Record Published” has green tick , hence this is completely secure and not vulnerable.

Case-II

Here as you can see, there is the line “Your email service provider is Proofpoint” , hence it is an email domain, and here as you can see “DMARC Policy Enabled” has a yellow
tick, which means, DMARC Policy is there but has not been properly enabled (i.e. p=none), so still chances of spoof emails to come into the inbox. So this is vulnerable and 
worth reporting. On Bugcrowd it’s VRT is “Server Security Misconfiguration > Mail Server Misconfiguration > No Spoofing Protection on Email Domain”. This is a P3 vulnerability
but is also given as P4 sometimes depending from program to program.

Case-III
Here as you can see, there is the line “Your email service provider is Google Apps” , hence it is an email domain, and here as you can see “DMARC Record Published” has red 
cross, hence there is no DMARC record for that domain, so spoof emails to come into the inbox. So this is vulnerable and worth reporting. On Bugcrowd it’s VRT it is same as
above “Server Security Misconfiguration > Mail Server Misconfiguration > No Spoofing Protection on Email Domain”. This is a P3 vulnerability but is also given as P4 sometimes
depending from program to program.

Case-IV

Here as you can see there is no line “Email Service Provider is…” , hence it is a non-email domain, so not worth reporting, the reason is that if the given email is not even an
email domain so it won’t matter if it has spoofing protection or not, as either way it isn’t being used for mailing purpose. So it vulnerable but not worth reporting , as no 
impact is there. In Bugcrowd VRT it is “Server Security Misconfiguration > Mail Server Misconfiguration > No Spoofing Protection on Non-Email Domain”, which is P5 vulnerability


Refer : https://medium.com/techiepedia/how-to-report-dmarc-vulnerabilities-efficiently-to-earn-bounties-easily-f7a65ecdd20b
