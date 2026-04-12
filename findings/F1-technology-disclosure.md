F1 — Technology Stack Disclosure

**Date:** 10 April 2026
**Tool:** Nmap
**Command:**
nmap -sV -sC -p 5050,5173,8545 192.168.1.104

**Raw output:**
5050/tcp open http Node.js Express framework

**What this means:**
Port 5050 openly identifies the backend as Node.js Express 
framework. This was identified without any authentication 
or credentials.
