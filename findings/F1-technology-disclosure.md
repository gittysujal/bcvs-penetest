F1 — Technology Stack Disclosure

Date:10 april 2026 
 tools:Nmap  
Command:
sudo nmap -sV -sC -p- -T4  192.168.1.104
 

Finding:
Nmap scan report for 192.168.1.104
Host is up (0.0086s latency).
Not shown: 65530 closed tcp ports (reset)
PORT      STATE SERVICE VERSION
5000/tcp  open  rtsp
| fingerprint-strings: 
|   FourOhFourRequest: 
|     HTTP/1.1 403 Forbidden
|     Content-Length: 0
|     Server: AirTunes/935.7.1
|     X-Apple-ProcessingTime: 2
|     X-Apple-RequestReceivedTimestamp: 124783417
|   GetRequest: 
|     HTTP/1.1 403 Forbidden
|     Content-Length: 0
|     Server: AirTunes/935.7.1
|     X-Apple-ProcessingTime: 1
|     X-Apple-RequestReceivedTimestamp: 124778374
|   HTTPOptions: 
|     HTTP/1.1 403 Forbidden
|     Content-Length: 0
|     Server: AirTunes/935.7.1
|     X-Apple-ProcessingTime: 1
|     X-Apple-RequestReceivedTimestamp: 124783403
|   RTSPRequest: 
|     RTSP/1.0 403 Forbidden
|     Content-Length: 0
|     Server: AirTunes/935.7.1
|     X-Apple-ProcessingTime: 1
|     X-Apple-RequestReceivedTimestamp: 124778398
|   SIPOptions: 
|     RTSP/1.0 403 Forbidden
|     Content-Length: 0
|     Server: AirTunes/935.7.1
|     CSeq: 42 OPTIONS
|     X-Apple-ProcessingTime: 1
|_    X-Apple-RequestReceivedTimestamp: 124783432
5050/tcp  open  http    Node.js Express framework
7000/tcp  open  rtsp
|_irc-info: Unable to open connection
| fingerprint-strings: 
|   FourOhFourRequest: 
|     HTTP/1.1 403 Forbidden
|     Content-Length: 0
|     Server: AirTunes/935.7.1
|     X-Apple-ProcessingTime: 1
|     X-Apple-RequestReceivedTimestamp: 124783363
|   GetRequest: 
|     HTTP/1.1 403 Forbidden
|     Content-Length: 0
|     Server: AirTunes/935.7.1
|     X-Apple-ProcessingTime: 2
|     X-Apple-RequestReceivedTimestamp: 124783332
|   HTTPOptions: 
|     HTTP/1.1 403 Forbidden
|     Content-Length: 0
|     Server: AirTunes/935.7.1
|     X-Apple-ProcessingTime: 1
|     X-Apple-RequestReceivedTimestamp: 124783348
|   RTSPRequest: 
|     RTSP/1.0 403 Forbidden
|     Content-Length: 0
|     Server: AirTunes/935.7.1
|     X-Apple-ProcessingTime: 2
|     X-Apple-RequestReceivedTimestamp: 124778357
|   SIPOptions: 
|     RTSP/1.0 403 Forbidden
|     Content-Length: 0
|     Server: AirTunes/935.7.1
|     CSeq: 42 OPTIONS
|     X-Apple-ProcessingTime: 3
|_    X-Apple-RequestReceivedTimestamp: 124783376
50510/tcp open  unknown
63919/tcp open  unknown
2 services unrecognized despite returning data. If you know the service/version, please submit the following fingerprints at https://nmap.org/cgi-bin/submit.cgi?new-service :
==============NEXT SERVICE FINGERPRINT (SUBMIT INDIVIDUALLY)==============
SF-Port5000-TCP:V=7.95%I=7%D=4/10%Time=69D8B649%P=aarch64-unknown-linux-gn
SF:u%r(GetRequest,8F,"HTTP/1\.1\x20403\x20Forbidden\r\nContent-Length:\x20
SF:0\r\nServer:\x20AirTunes/935\.7\.1\r\nX-Apple-ProcessingTime:\x201\r\nX
SF:-Apple-RequestReceivedTimestamp:\x20124778374\r\n\r\n")%r(RTSPRequest,8
SF:F,"RTSP/1\.0\x20403\x20Forbidden\r\nContent-Length:\x200\r\nServer:\x20
SF:AirTunes/935\.7\.1\r\nX-Apple-ProcessingTime:\x201\r\nX-Apple-RequestRe
SF:ceivedTimestamp:\x20124778398\r\n\r\n")%r(HTTPOptions,8F,"HTTP/1\.1\x20
SF:403\x20Forbidden\r\nContent-Length:\x200\r\nServer:\x20AirTunes/935\.7\
SF:.1\r\nX-Apple-ProcessingTime:\x201\r\nX-Apple-RequestReceivedTimestamp:
SF:\x20124783403\r\n\r\n")%r(FourOhFourRequest,8F,"HTTP/1\.1\x20403\x20For
SF:bidden\r\nContent-Length:\x200\r\nServer:\x20AirTunes/935\.7\.1\r\nX-Ap
SF:ple-ProcessingTime:\x202\r\nX-Apple-RequestReceivedTimestamp:\x20124783
SF:417\r\n\r\n")%r(SIPOptions,A1,"RTSP/1\.0\x20403\x20Forbidden\r\nContent
SF:-Length:\x200\r\nServer:\x20AirTunes/935\.7\.1\r\nCSeq:\x2042\x20OPTION
SF:S\r\nX-Apple-ProcessingTime:\x201\r\nX-Apple-RequestReceivedTimestamp:\
SF:x20124783432\r\n\r\n");
==============NEXT SERVICE FINGERPRINT (SUBMIT INDIVIDUALLY)==============
SF-Port7000-TCP:V=7.95%I=7%D=4/10%Time=69D8B64E%P=aarch64-unknown-linux-gn
SF:u%r(RTSPRequest,8F,"RTSP/1\.0\x20403\x20Forbidden\r\nContent-Length:\x2
SF:00\r\nServer:\x20AirTunes/935\.7\.1\r\nX-Apple-ProcessingTime:\x202\r\n
SF:X-Apple-RequestReceivedTimestamp:\x20124778357\r\n\r\n")%r(GetRequest,8
SF:F,"HTTP/1\.1\x20403\x20Forbidden\r\nContent-Length:\x200\r\nServer:\x20
SF:AirTunes/935\.7\.1\r\nX-Apple-ProcessingTime:\x202\r\nX-Apple-RequestRe
SF:ceivedTimestamp:\x20124783332\r\n\r\n")%r(HTTPOptions,8F,"HTTP/1\.1\x20
SF:403\x20Forbidden\r\nContent-Length:\x200\r\nServer:\x20AirTunes/935\.7\
SF:.1\r\nX-Apple-ProcessingTime:\x201\r\nX-Apple-RequestReceivedTimestamp:
SF:\x20124783348\r\n\r\n")%r(FourOhFourRequest,8F,"HTTP/1\.1\x20403\x20For
SF:bidden\r\nContent-Length:\x200\r\nServer:\x20AirTunes/935\.7\.1\r\nX-Ap
SF:ple-ProcessingTime:\x201\r\nX-Apple-RequestReceivedTimestamp:\x20124783
SF:363\r\n\r\n")%r(SIPOptions,A1,"RTSP/1\.0\x20403\x20Forbidden\r\nContent
SF:-Length:\x200\r\nServer:\x20AirTunes/935\.7\.1\r\nCSeq:\x2042\x20OPTION
SF:S\r\nX-Apple-ProcessingTime:\x203\r\nX-Apple-RequestReceivedTimestamp:\
SF:x20124783376\r\n\r\n");
MAC Address: B2:D7:9B:42:A1:37 (Unknown)

Service detection performed. Please report any incorrect results at https://nmap.org/submit/ .
Nmap done: 1 IP address (1 host up) scanned in 873.31 seconds

Port 5050 openly identifies the backend as Node.js Express framework.
No authentication required to fingerprint the service.

Evidence:
5050/tcp open http Node.js Express framework

what this means
The service on port 5050 reveals it is running Node.js Express. 
This was identified without any authentication or credentials.
