### Common exploits
- kerberos roasting
    - This is where we can take the domain and user name (SPN) and try to get a TGT (Ticket Granting ticket) We can then attempt to crask the hash to get the user password (This will be exachnegd in the kerberos authenticaiton)
 
#### asperosting
```
GetNPUsers <domain> -dc.ip $target -usersfile <filename> -outfile <filename>
```
