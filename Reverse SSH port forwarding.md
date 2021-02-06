Reverse SSH port forwarding specifies that the given port on the remote server host is to be forwarded to the given host and port on the local side.

A problem rises when we try to connect to a remote server that is behind a firewall and that firewall rejects any incoming connections. 
Simply put, you want to connect your local machine to a server, so that you can use the tunnel to connect from the server to your local machine.


If a site was blocked, you can forward the traffic to a server you own and view it. For example, if imgur was blocked at work, you can do:
```
	ssh -L 9000:imgur.com:80 user@example.com
```
Going to localhost:9000 on your machine, will load imgur traffic using your other server.

The -R flag is a remote tunnel (YOU --> CLIENT). You forward your traffic to the other server for others to view. Similar to the example above, but in reverse.

