**Design and Implementation of a Bank System Network Design**  

**Introduction**  
As part of a team of final-year students, I designed and implemented a scalable, secure, and efficient enterprise network to support their four-story headquarters. This project leveraged **OSPF, VLANs, Inter-VLAN Routing, DHCP, SSH, and Wireless LANs** to ensure seamless communication across departments and robust security.  

---

**Network Design**  

1️⃣ **Infrastructure**  
- **Access Switches**: Deployed across departments (VLANs 10, 20, 30, etc.), supporting 60+ wired/wireless users each.  
- **Multilayer Switches**: Configured with **Switch Virtual Interfaces (SVI)** for Inter-VLAN routing.  
- **Routers**: Interconnected via **OSPF** for dynamic routing and **SSH** for secure remote access.  
- **Wireless Access Points**: Integrated into each department for wireless connectivity.  
- **Server Room**: Hosted dedicated **DHCP, HTTP, and Email servers** for centralized services.  

---

2️⃣ **Connectivity & Protocols**  
- **VLANs & Subnetting**:  
  - Base IP: **192.168.10.0** subnetted for departments, server room, and wireless networks.  
  - Calculated subnet masks, usable IP ranges, and broadcast addresses for each VLAN.  
- **Dynamic Routing**:  
  - **OSPF** advertised routes across the network, ensuring backbone (Area 0) connectivity.  
- **DHCP**:  
  - Hosts dynamically assigned IPs from the server room’s DHCP pool.  
- **Wireless Configuration**:  
  - Cisco Access Points deployed per department with SSID and WPA2 security.  

---

3️⃣ **Security & Services**  
- **SSH**: Configured on all routers for encrypted remote management.  
- **Port-Security**: Enabled on switches using **sticky MAC addresses** and violation shutdown.  
- **Servers**:  
  - **HTTP Server**: Hosted internal banking portals.  
  - **Email Server**: Enabled secure communication.  
- **Device Hardening**:  
  - Set hostnames, console/enable passwords, banners, and encrypted all credentials.  
  - Disabled IP domain lookup to prevent unnecessary delays.  

---

**Network Testing**  
✅ **Ping Tests**: Verified inter-VLAN and inter-department connectivity.  
✅ **OSPF Validation**: Used `show ip ospf neighbor` and `show ip route` to confirm route advertisements.  
✅ **DHCP Checks**: Ensured devices received correct IPs from the server room.  
✅ **SSH Access**: Tested secure login to routers.  
✅ **Port-Security**: Triggered violations to validate shutdown of unauthorized devices.  

---

**Conclusion & Acknowledgments**  
This project deepened my expertise in enterprise network design, emphasizing scalability, security, and compliance with banking-sector requirements. Successfully implementing OSPF, VLANs, and centralized DHCP highlighted the importance of hierarchical design in large-scale environments.  

Special thanks to my team and faculty mentors for their guidance!  

**Tools Used**: Cisco Packet Tracer  
**Topology**: Verified and fully functional 

<br />


<h2>Packet Tracer Image</h2>


<p align="center">
Packet Tracer: <br/>
<img src="https://i.imgur.com/TGJGRCu.png" height="80%" width="80%" alt="bank Network"/>
<img src="https://i.imgur.com/sleUkr0.png" height="80%" width="80%" alt="bank Network"/>
<img src="https://i.imgur.com/Fpm1D1o.png" height="80%" width="80%" alt="bank Network"/>
<img src="https://i.imgur.com/54I0E5o.png" height="80%" width="80%" alt="bank Network"/>
<img src="https://i.imgur.com/gekIOua.png" height="80%" width="80%" alt="bank Network"/>
<img src="https://i.imgur.com/gQKKfQv.png" height="80%" width="80%" alt="bank Network"/>



<br />

#Networking #OSPF #Cybersecurity #Cisco #DHCP #VLAN #EnterpriseNetworking #ITInfrastructure  
