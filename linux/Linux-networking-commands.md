# Linux Networking 

## Interface & IP address commands

### ipaddr
- Shows all network interfaces and their IP addresses
- Used to check system's IP address, to verify if an interface is UP or DOWN, to see subnet masks

### ip a
- Shortcut of ip addr

### ip addr show
- Same as ip addr/ip a

### ifconfig
- Deprecated, shows all network interfaces and their IP addresses

### hostname
- Displays the system hostname (stored in /etc/hostname) inside the network

### hostname -I
- Displays only ip address(es) of the system
- If your system has multiple intrfaces you will see multiple ips

## Connectivity testing commands

### ping
- Tests network connectivity between your system and a destination
- It tells whether destination is reachable, round-trip time (latency), packet loss percentage, DNS resolution (if using domain name)

### traceroute
- It shows hop-by-hop routers your packet takes to reach destination

## DNS commands

### nslookup
- DNS query tool, queries a DNS server to resolve a domain name into an IP address

### dig
- Domain Information Grouper
- It is a powerful DNS troubleshooting tool, gives more detailed DNS response information

### host
- It is a simple DNS lookup tool
