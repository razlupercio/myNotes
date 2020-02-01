# General TCP & UDP enumeration

2020-02-01

nmap  --top-ports 100 --open -iL iplist.txt
nmap -sS -A -sV -O -p- ipaddress
nmap -sU ipaddress
nmap –sV -v -n --script vuln ipaddress 
nmap --script ssl-heartbleed ipaddress 

