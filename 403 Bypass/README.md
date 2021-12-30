### How to Bypass 403 restrictions?
There are many headers and paths which you can use to bypass 403 restrictions.
1.Adding in URL Paths: Adding this in paths of the URL and the file which is forbidden
/*
/%2f/
/./
/
/*/
2.Adding Headers in request :By adding different headers in request with value 127.0.0.1 can also help in bypassing restrictions.
X-Custom-IP-Authorization
X-Forwarded-For
X-Forward-For
X-Remote-IP
X-Originating-IP
X-Remote-Addr
X-Client-IP
X-Real-IP
Reference: https://github.com/yunemse48/403bypasser
3. Changing the request method type: Changing method from GET to POST , etc can also lead to bypass.
Reference: 
 * https://infosecwriteups.com/403-forbidden-bypass-leads-to-hall-of-fame-ff61ccd0a71e
 * https://sapt.medium.com/bypassing-403-protection-to-get-pagespeed-admin-access-822fab64c0b3
