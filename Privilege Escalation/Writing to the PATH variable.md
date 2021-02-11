We can write to the \$PATH variable so that when a program calls another executable it will run our executable instead of a system one.

We write our own executable and add it to the PATH variable:
```**"export PATH=/tmp:$PATH"**```