

```
snmpwalk -v2c -c public $target

snmpwalk -v1 -c public $target > snmp.txt
```



```
sudo apt install onesixtyone

onesixtyone -c /opt/useful/seclists/Discovery/SNMP/snmp.txt $target
```

```
sudo apt install braa
braa <community string>@$target:.1.3.6.*   # Syntax

braa public@$target:.1.3.6.*
```

