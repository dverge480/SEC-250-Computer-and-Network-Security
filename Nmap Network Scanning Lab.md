# Nmap Network Scanning Lab

This lab shows how to port scan using Nmap.

### Notes
Start Apache and MySQL services using XAMPP to ensure your webserver is running.
Verify by accessing http://localhost/web1.html or any other page hosted on your localhost.
Configure Network Accessibility:

If necessary, adjust or temporarily disable your firewall to allow network access to your web pages.

### Install Nmap:

Download the latest stable release of Nmap
Install using the default options.
Network Scanning:

### Ping Scan:

Open Zenmap as administrator.
Set the target range (e.g., 192.168.1.1-254 for a 192.168.1.X network).
Select the "Ping Scan" profile and start the scan.


![image](https://github.com/user-attachments/assets/8cdb6866-8ee1-455b-aed3-eed7d71dfd8a)


### Open Ports Scan:

Select three hosts within your network as targets.
Choose "Quick scan plus" profile.
Note the Nmap command issued and research the options used (excluding -version-light).

Take note of information:

a. 192.168.1.30
b. Open ports: 1 
c. Running services: 1
d. OS guess: HP ProCurve 1810G
e. Number of filtered ports: 0
f. Number of closed ports: 99

a. 192.168.1.31
b. Open ports: 1 
c. Running services: 1
d. OS guess: None
e. Number of filtered ports: 0
f. Number of closed ports: 99


a. 192.168.1.141
b. Open ports: 1
c. Running services: 1
d. OS guess: HP ProCurve 1810G
e. Number of filtered ports: 0
f. Number of closed ports: 99



Use the same targets for an "Intense Scan plus UDP".
This scan reveals more information about hosts.
