## Project Overview- Week 2
This project demonstrates a TCP/IP network setup using GNS3 with multiple hosts connected through a switch. Each host is configured with a static IP address and tested using ping commands.

---

## Network Topology
- 4 Hosts (Host1, Host2, Host3, Host4)
- 1 Switch
- Star topology connection

---

## IP Configuration

| Host  | IP Address |
|------|-----------|
| Host1 | 10.10.2.1 |
| Host2 | 10.10.2.2 |
| Host3 | 10.10.2.3 |
| Host4 | 10.10.2.4 |

Subnet Mask: 255.255.255.0

---

## Configuration Code

```bash
auto eth0
iface eth0 inet static
    address 10.10.2.X
    netmask 255.255.255.0
    up echo nameserver 192.168.0.1 > /etc/resolv.conf
```

---

## Screenshots

### Topology
![Topology](topology.png)

### Host 1 Configuration
![Host1](configh1.png)

### Host 2 Configuration
![Host2](configh2.png)

### IP Address Host1
![IP1](h1ipaddres.png)

### IP Address Host2
![IP2](h2ipaddres.png)

### IP Address Host3
![IP3](h3ipaddress.png)


### Console Host3
![Console3](h3console.png)

### Console Host4
![Console4](h4console.png)

### Ping Test (Success Host1 to Host2)
![Ping1](ping1to2.png)

### Ping Test (Success Host4 to Host2)
![Ping2](ping-sucess4to2.png)

### Ping Test (Failure)
![Failure](h1pingfailed.png)

