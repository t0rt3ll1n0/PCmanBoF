# PCman FTP Server Buffer overflow > internal DoS [CVE-2013-4730]
A very simple buffer overflow using CVE-2013-4730 against PCman's FTP server
## How it works?
A very simple Buffer overflow that overwrite both the buffer and the EIP
## Can i obtain a RCE?
Yes, simply use a shellcode after the ````"A"*2004```` and it will be executed after overwriting
Of course launch ````nc -lvp 4444````
I advise to use a bind shell instead a reverse shell

