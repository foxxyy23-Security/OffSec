## scanning
```
sudo nmap $target -sV -sC -p3306 --script mysql*
```
## connecting to service
```
mysql -u <username> -p<password> -h $target
```
## Database commmands:
```
mysql> use sys;
mysql> show tables;  
mysql> select host, unique_users from host_summary;

```
