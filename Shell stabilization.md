```
python -c 'import pty; pty.spawn("/bin/bash")'
export TERM=xterm
```

ctrl + Z to bg the shell and then:

```stty raw -echo; fg```
