# Validation Tests

## 1. DHCP Verification

Command:
ipconfig /all

Expected:
- IP address in 172.16.0.x range
- DNS: 172.16.0.10
- Gateway: 172.16.0.10

![DHCP verification](screenshots/35.0-dhcp-verification.png)


---

## 2. Domain Join

Test:
System joined to domain: lab.local

Expected:
Login with domain account works

![Domain join succeded](screenshots/35.1-domain-join.png)


---

## 3. DNS Resolution

Command:
nslookup lab.local

Expected:
Returns DC01 IP address

![DNS resolution](screenshots/35.2-dns-resolution.png)


---

## 4. Network Connectivity

Command:
ping 172.16.0.10

Expected:
Successful reply

![Network connectivity](screenshots/35.3-network-connectivity.png)


---

## 5. Internet Access

Command:
ping 8.8.8.8

Expected:
Successful reply via RRAS NAT

![Internet access](screenshots/35.4-internet-access.png)
