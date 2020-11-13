# PCman FTP Server Buffer overflow > internal DoS [CVE-2013-4730]
A very simple buffer overflow using CVE-2013-4730 against PCman's FTP server
## How it works?
You have to modify if for internal DoS, try using a while loop to send bigger and bigger packages. The badchar var is for test and it might be modified

## Can i obtain a RCE?
Yes, simply use a shellcode after the ````"A"*2004```` and it will be executed after overwriting
Of course launch ````nc -lvp 4444````
I advise to use a bind shell instead a reverse shell

