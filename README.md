# Lab 1:. Small Enterprise Network with VLANs, Inter-VLAN Routing, and DHCP

# Lab Overview:
Over the past week, I completed a practical networking lab using Cisco Packet Tracer to strengthen my understanding of real-world network design and configuration. 
In this project, I designed and configured a small enterprise-style network with (1) Multiple VLANs (network segmentation), (2) Inter-VLAN routing using Router-on-a-Stick and 
(3) DHCP services for automatic IP address assignment.

# Software & Devices Used:
- Cisco Packet Tracer (Software)  
- Router (1)  
- Switch (1)  
- Personal Computers (6)  

# Procedure
# Part 1 (Initial Configs)
- Place and Connect Devices  
- Name and Secure Switch  
- Name and Secure Router  
- Give IP address to Router  
- Enable ports on Router  
- Give static IP addresses to PCs  
- Test Connectivity  
#
# Part 2 (Create and Configure VLANs)
- Check VLAN status  
- Draft VLAN topology  
- Create and Name VLANs  
- Assign VLANs to interfaces  
- Create Trunk port  
- Test Connectivity (pinging devices in other VLANs should fail)  
(Purpose: Segment the network into separate broadcast domains for better performance and security.)  
#
# Part 3 (ROAS)
- Confirm interfaces for trunk  
- Create sub-interfaces on Router  
- Change default gateways of PCs to sub-interface IP address  
- Test Connectivity  
(Purpose: Enable communication between VLANs using a single router interface.)  
#
# Part 4 (DHCP)  
- Confirm IP addresses to exclude  
- Exclude IP addresses  
- Create DHCP pool  
- Create DHCP pool range  
- Establish default router  
- Set DNS to Google's DNS server  
- Change all PCs IP configuration to DHCP (auto)  
- Test Connectivity  
(Purpose: Automate IP address assignment and reduce manual configuration errors.)
#
# Takeaways and Challenges 
A few things went wrong during this lab. I had a few Coding errors such as  (1) excluding the default gateway from EVERYTHING else. (I forgot to exclude it from DHCP and also fmistakely used it as end deveice IP address).
Another coding error I had was (2) when creating the sub-interfaces for R1, I tried to assign an IP address first instead of establishing the Encapsulation is _802.1Q_. This resulted in the sub-interfaces not being up.  

# Skills Learned:  

- VLAN creation and network segmentation  
- Switch port configuration (access vs trunk)  
- Inter-VLAN routing (Router-on-a-Stick)  
- DHCP configuration for multiple networks  
- IP addressing and subnetting fundamentals  
- Network troubleshooting using CLI commands

# Images:  
1.Schematic
<img width="993" height="893" alt="1_Diagram" src="https://github.com/user-attachments/assets/4f0d6c40-48c5-4a12-b4da-11787f86472a" />  

2. Initial Configurations  
<img width="1374" height="1055" alt="2_Initial Config" src="https://github.com/user-attachments/assets/62148c37-401a-4f65-9fe9-908ea9a04edf" />

3. VLAN Configurations
<img width="1165" height="986" alt="3_VLANs" src="https://github.com/user-attachments/assets/3fa761ae-2627-4a8b-ac87-4d96183368c2" />

4. Inter-VLAN routing (ROAS)
<img width="985" height="825" alt="4_ROAS" src="https://github.com/user-attachments/assets/9b16435e-d16f-4395-9044-eeb5e134aad0" />

5. DHCP Configuration
<img width="1098" height="1065" alt="5_DHCP" src="https://github.com/user-attachments/assets/59a3ba4c-2c00-4179-8827-d82ab1cc6bdd" />

6. Test Connectivity using 'ping' command from PC0
<img width="1023" height="1140" alt="6_Test ping" src="https://github.com/user-attachments/assets/ee833d57-99f4-4ed9-8137-c2ef10838851" />

7. Screenshot of "Encapsulation error"
<img width="1481" height="1212" alt="7_error1" src="https://github.com/user-attachments/assets/4bccaa8c-71c2-454e-bda6-8454cb6c5058" />





  

















