Basic directory enum command
```gobuster dir -u http://<ip>:3333 -w <word list location>```
 
 **dir** uses directory/file brutceforcing mode.
**-u** specify url.
**-w** specify wordlist.
**-o** output file.
**-x** specify extension.
**-c** specify a cookie.

DNS subdomain enumeration:
```
gobuster dns -d <domain> -w ~/Documents/basics/subdomains-10000.txt -i
```

