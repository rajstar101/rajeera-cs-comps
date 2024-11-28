# rajeera-cs-comps
website link: https://www.cs.carleton.edu/cs_comps/2425/security/Yeabsira-Rajeera/

^^^ website include: video tutorial and refrences
---

# ARP Poisoning and MITM Attack Simulation

## Project Overview

This project illustrates how an ARP poisoning attack can be executed as part of a Man-in-the-Middle (MITM) attack, highlighting vulnerabilities in network protocols. The simulation modifies the target's ARP cache to intercept, monitor, and manipulate network traffic. It emphasizes the importance of detecting ARP spoofing and employing network encryption to safeguard data integrity and privacy.

---

## About the Developers

- **Names**: Rajeera Geleta and Yeabsira Gebreegziabher
- **Adviser Professor**: Jeff Ondich  

---

## Resources

1. Project Proposal
2. arp.c

---

## How to use?

1. **Clone the repository**

2. **Install dependencies** (listed on top of the source code):

3. **Set up a NAT-configured network**
   - Configure a network with two virtual machines for ARP poisoning.
     *in our case*
     - We used VMware to create the virtual machines and network.
     - Our virtual machines ran on kali and linux mint.

5. **Compile the source code**

6. **Run the program**:  
   Execute the program with the appropriate parameters:  
   sudo ./arp <interface> <your_mac> <target_ip>
   Replace ...
   - <interface> with network interface (eth0 was used in our example)
   - <your_mac> with the MAC address of your machine (the one your hacking from).
   - <target_ip> with the IP address of the machine your victim is communicating with (we targeted the "router" in our case).

---

## Source Code

Key features of the source code:
- Generates and transmits spoofed ARP packets.
- Alters the ARP cache of the victim device to redirect its traffic to the attacker’s machine.
- Utilizes raw sockets for detailed control over packet manipulation.

---

# Disclaimer

This project is intended for educational purposes only. Unauthorized use of ARP poisoning techniques is illegal and unethical.

--- 
