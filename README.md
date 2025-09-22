# Task-1-Scan-Your-Local-Network-for-Open-Ports
Cyber Security Internship
# Install Nmap 
We install nmap from official website (or) used nmap for Kali linux virtual machine.

# Finding IP range
Normal to finding we used ipconfig in windows and ifconfig in linux.Now we know your ipaddress eg:192.168.1.0/24 (or) 10.128.129.0/24.It means we using class C ip range.The C class is for first three bytes for constant and four byte is changing.
[1 byte = 8 bit] [1 bit = 0(or)1] [0/24 means first three bytes are fulled.]
Form knowing ip address is ifcongig in kali linux.
Now we know ipaddress.
ip address : 10.128. . .

# Nmap
Nmap is a  port scanning tools for open ports on IPaddress.It useful for active reconnaissace tool it means we directly connecting to victims(or) ip address.
Example : Saying hii to other person it means hey I am here.
Nmap is used scan my own ipaddress to find open ports.
we used nmap -sS ipaddress
example : 433 service tcp
          53 service dns
          Mac address of system
This scan is send TCP SYN request to system where the system never denail it.The system thinks like hey, haa I am there.So this scan is for active reconnaissance.

# Nmap Using with our ip address
In nmap there so many scans are avaliable.But we using -sS for TCP SYN scan it for knowing open ports in system.
It display opens ports with services is running with them.

# Wireshark
Wireshark is used for packet capturing and packet analyze tool.In wireshark it display source ip address,destination ip address,ports,protocol and packer size ect.
Comman port are https,tcp,http,dns ect.

# Open port with services
Open ports with services means one service is have port number.
Example : HTTPS is 433
          DNS is 53
          HTTP is 80
          FTP is 20/21
          SMTP is 25
          SSH is 22

# Security risks from open ports
Risks is there from open ports how means in ipaddress(or)victims SSH service is open it means remote login is possible with port 22.
HTTP sevice is open it means data is transering without encapsulation.Then data is vissble in wireshark(or) tools.
To avoid this is use firewall,honeypots and proxy to mange it.
# Firewall
In firewall there IDS and TPS for blocking or pervent for scannings.It works like wall between request and receive traffic.Firewall is monitoring and filter traffic of network.

