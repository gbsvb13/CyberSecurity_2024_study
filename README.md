# CyberSecurity_2024_study
this txt file is my archive of studying cybersecurity- 2024.09.03 started.

cybersecurity divided into two species, Offensive Security and Defensive Security.
Offensive Security is focused on breaking into system. it can be achieved by exploiting/abusing insecure setups and taking adventage of unenforced access control policies.

Defensive Security's two main tasks 
1.Preventing intrusions from occurring
2.Detecting intrusions when they occur and responding properly

0904
Devices on the Internet are identified by their ip adresses and MAC addresses - MAC addresses are similar with serial num.
Protocols : IP address' s set of standards
IP : Internet Protocol
IP addresses can change from device to device but cannot be active simultaneously more than once within the same network.

public ip address are used to identify device on the internet / private ip address are used to identify a device from other devices.
public ip addresses are given by ISP(Internet Service Provider) at a monthly fee

if ip address looks 127.0.0.1 : ipv4
if it looks 2a00:22c4:a531:c500:425f:cce6:c36b:f64d -> ipv6

MAC address : device's physical network interface(probably microchip).
network interface is assigned a unique address at the factory it was built at, called a MAC (Media Access Control ) address

how MAC address looks like:
ex) a4:c3:f0:85:ac:2d
first six characters represent the company that made the network interface, and the last six is a unique number.

but MAC address can be faked or spoofed and the spoofed MAC address can deceive firewall.

Ping used determine the performance of a connection between devices.
Ping measures ICMP(Internet Control Message Protocol)'s travelling time to travelling another device by measuring time of ICMP's echo packet and ICMP's echo reply from the target device.

0905
The idea of web application : a program running on a remote server.

0907
Web application's security risks
Identification and Authentication Failure:
allowing brute force/storing user's ps in plain texts/weak passwords

Broken Access control
meaning: an attacker can access information or perform actions not intended for them 
vulnerabilities : giving users more access permissions than they need/
IDOR : Insecure Direct Object References
ex) a photo named 1020, then attacker can access a photo named 1021 or 1022

injection
make attaker can inject malicious code into web code
Cause : lack of proper validation and sanitization of user's input

Cryptographic failures
*key of Cryptography: encrypte the data and make it look gibberish who doesn't have a key
Use HTTP not HTTPS : HTTPS is secured version of HTTP.
Relying on a weak cryptographic algoritm
using dafault or weak keys. ex)1q2w3e4r

DNS
DNS : Domain Name System
Domain names are IP address.

Domain Hierarchy
TLD : Top-Level Domain
Root Domain : .
Top-lelve Domain : .edu, .com, .gov, .mil
Second-name domain : etc.

TLD divided by two, gTLD(generic top level) and ccTLD(country code top level domain).
gTLD used its domain name for their commercial perpose. ex).org : organization
ccTLD used for geographical purposes. ex).ca : canada.
but there's new gTLDs ranging from .online/.club etc.

In Tryhackme.com , .com is top level domain and Tryhackme is second level domain.
the second level domain cannot start with hyphens or consecutive hyphens.
if admin.tryhackme.com, admin is subdomain part.

DNS Record Types
A Record : Recording ipv4 addresses
AAAA Record : Recording ipv6 adresses
CNAME Record : resolve to another domain name
MX Record : resolve to the address of the servers that handle the email for the domain you are querying.
Txt Record : Free text fields. any text-based data can be restored. used commonly list servers and signing up for third party services.





