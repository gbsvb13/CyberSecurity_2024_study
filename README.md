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

240909
URL : Uniform Resource Locater.
its instruction of how to access a resource on the internet.
URL is composed to; Scheme, User, Host, Port, Path, Query String, Fragment. (it doesn't use all features in every request)

Methods of HTTPs

GET request : getting information from the web server
POST request : used submittiong data to the web server and creating new records(potentially)
PUT request : used for submittiong data to a web server to update data
DELETE request : deleting information from a web server

HTTP's status codes
100 ~ 199 : first part of request is completed and should continue sending the rest of their request. no longer appears in normal situations.
200 ~ 299 : request was successfully completed.
300 ~ 399 : telling clinent to go another resource.
400 ~ 499 : Clinet Errors. there is a error with client's request. ex) 404 not found
500 ~ 599 : Server Errors. server side's error occured.

Common HTTP status codes:
200 : OK
201 : Created (resource has been created)
301 : redirection to new webpage *webpage's information transferred.
302 : Found. 
400 : Bad Request - Something was either wrong or missing in their request. This could sometimes be used if the web server resource that is being requested expected a certain parameter that the client didn't send.
401 : Not Authorised -

1002
How website works
Browser -> Request from browser(through Internet) -> server -> response from server -> internet -> Browser
--> website works with Trade of requests between browser and server with internet.
client side : Frontend / Server side : Backend.

construction of website : html / Css / JavaScript.
HTML and CSS are used for static website (not interaction with user)
dynamic website : Javascript.(Interaction with user)

In the test level in website, there might be a admin password or id in the website's source code. 
if you can find it, you can invade website.

HTML Injection is a vulnarability that occurs when unfiltered user input is displayed on the page.
