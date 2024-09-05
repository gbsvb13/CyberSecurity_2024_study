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
