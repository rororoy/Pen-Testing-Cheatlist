We can use SQL Map with a captured HTTP request from burp. Once the request is captured, write it to a text file. Now we run 
```sqlmap -r request.txt --dbms=mysql --dump```

**--dbms** is the type of the data base.
**--dump** tells us to dump the whole DB.