  GNU nano 8.6                                                     New Buffer *                                                            
Date: 11 April 2026
Tool: Gobuster + curl
Commands:  
gobuster dir -u http://192.168.1.104:5050 -w /usr/share/wordlists/dirb/common.txt --timeout 30s

curl -v http://192.168.1.104:5050/Health

Raw output:  
/health    (Status: 200) [Size: 11]
/Health    (Status: 200) [Size: 11]

{"ok":true}

What this means:  
The /health endpoint was discovered through directory bruteforcing.
It responds with server status to anyone with no authentication
required. Both /health and /Health work meaning the endpoint
is case insensitive
  
Command:curl -v http://192.168.1.104:5050/Health

Raw output:  
HTTP/1.1 200 OK
Access-Control-Allow-Origin: http://localhost:5173

What this means:     
Despite CORS policy restricting to localhost:5173, the health
endpoint returns 200 OK to requests from any origin including
evil.com. No authentication required. Accessible from any
machine on the network.
