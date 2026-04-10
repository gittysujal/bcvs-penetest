Date: 10 April 2026  
Tool: curl  
Commands run:
curl -v http://192.168.1.104:50510/
curl -v http://192.168.1.104:63919/

Raw output
  curl -v http://192.168.1.104:50510/               
*   Trying 192.168.1.104:50510...
* Connected to 192.168.1.104 (192.168.1.104) port 50510
* using HTTP/1.x
> GET / HTTP/1.1
> Host: 192.168.1.104:50510
> User-Agent: curl/8.15.0
> Accept: */*
> 
* Request completely sent off
 * Empty reply from server
* shutting down connection #0
curl: (52) Empty reply from server
                                                                                                                                           
┌──(sujal㉿kali)-[~]
└─$ curl -v http://192.168.1.104:63919/
*   Trying 192.168.1.104:63919...
* Connected to 192.168.1.104 (192.168.1.104) port 63919
* using HTTP/1.x
> GET / HTTP/1.1
> Host: 192.168.1.104:63919
> User-Agent: curl/8.15.0
> Accept: */*
> 
* Request completely sent off


What this means:
Both ports are open and accepting TCP connections but do not 
respond to HTTP requests. These are not part of the BCVS 
application. Likely Mac OS background processes using 
non-HTTP protocols.

Conclusion:
Not exploitable via HTTP. No further investigation needed
