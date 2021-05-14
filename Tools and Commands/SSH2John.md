```python /usr/share/john/ssh2john.py id_rsa > id_rsa.hash```

```john id_rsa.hash --wordlist=/usr/share/wordlists/rockyou.txt```