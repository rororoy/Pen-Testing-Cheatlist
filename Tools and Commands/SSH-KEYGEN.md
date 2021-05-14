We can generate a key that will allow us to connect to a hosts machine through ssh:
 ```ssh-keygen -f <USERNAME TO LOGIN AS>```
 A .pub file will be created:
 ```cat file.pub``` & copy
 On the machine:
```echo '<THE PUB FILE>' > .ssh/authorized_keys```
On our machine:
```chmod 600 <THE OTHER FILE CREATED>```
```ssh -i <OTHER FILE> USERNAME@IP```	