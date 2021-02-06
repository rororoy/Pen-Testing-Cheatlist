Use **ss** to investigate sockets running on a host.
If we run ```ss -tulpn``` it will tell us what socket connections are running

**-t** to display TCP sockets.
**-u** to display UDP sockets.
**-l** to display only listening ports.
**-p** to show the procces using the port.