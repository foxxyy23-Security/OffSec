# 21 - FTP
- can be used with anonmyous login
## scanning port
```
sudo nmap -sV -p21 -sC -A $target --script ftp*
```

### helpful commands
- Trace
- Status's
- Debug
- get 
    - Downlaods files
- put
    - uploads files

### conncting to port
```
sudo ftp $target 

## if you have creds 
ftp <user>@$target

## if ftp on non-standard port 
ftp $target <port>
```

### downloading all files
- if you have creds, use following wget command to dump all files in the share
```
wget -m --no-passive ftp://anonymous:anonymous@$target
```
