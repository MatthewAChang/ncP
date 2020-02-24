# ncP

ncP is a C utility for reading and writing to TCP network connections. It is an implementation of Linux's netcat utility. ncP implements synchronous input and output between the server and its clients and can host up to 10 clients.

Usage: %s [-k] [-l] [-v] [-r]  [-p source_port] [-w timeout] [hostname] [port[s]]<br />
-k Forces nc to stay listening for another connection after its current connection is completed.<br />
-p source_port   Specifies the source port nc should use, subject to privilege restrictions and availability.<br />
-v Print more verbose output to standard error.<br />
-w timeout  If a connection and stdin are idle for more than timeout seconds, then the connection is silently closed.  The -w flag has no effect on the -l option.<br />
-r This option can only be used with the -l option. When this option is specified the server is to work with up to 10 connections simultaneously.<br />

Any data read from a network connection by the server is resent to all the other connections
