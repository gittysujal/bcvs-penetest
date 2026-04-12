
**Date:** 10 April 2026
**Tool:** curl
**Commands:**
curl -v http://192.168.1.104:50510/
curl -v http://192.168.1.104:63919/

**Raw output:**
* Empty reply from server
curl: (52) Empty reply from server

**What this means:**
Both ports accept TCP connections but do not respond to 
HTTP requests. Likely Mac OS background processes. 
Not exploitable via HTTP
