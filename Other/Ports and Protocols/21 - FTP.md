# 21 - FTP
- can be used with anonmyous login
### helpful commands

- get <filename>
- put <filename>

' sudo nmap -sV -p21 -sC -A $target '
### conncting to port
'sudo ftp $target 

##if you have creds 
ftp <user>@$target


## if ftp on non-standard port 
ftp $target <port>
'