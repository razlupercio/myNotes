# General TCP & UDP enumeration

2020-02-01


- [ ] check all ports
- 


## nmap

local network discovery

`nmap -sP 192.168.56.0/24`

`nmap -T4 -p- -A 192.168.56.102`

-p- = all ports
-A  = fingerprint all

```
nmap  --top-ports 100 --open -iL iplist.txt
nmap -sS -A -sV -O -p- ipaddress
nmap -sU ipaddress
nmap –sV -v -n --script vuln ipaddress 
nmap --script ssl-heartbleed ipaddress 
```

### nmap scripts

`ls -la /usr/share/nmap/scripts/ | grep smb`

`nmap -p139,445 --script=smb-enum-*`

## masscan 

https://github.com/robertdavidgraham/masscan

### useful links

https://danielmiessler.com/study/masscan/
