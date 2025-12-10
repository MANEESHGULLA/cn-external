# Peer-to-Peer Network Simulation in Cisco Packet Tracer

## **Aim**
To simulate a peer-to-peer network by directly connecting two PCs using a crossover cable and verify communication using Simulation Mode in Cisco Packet Tracer.

---

## **Description**
A peer-to-peer network allows two computers to communicate directly without using a switch or router. In Cisco Packet Tracer, two PCs can be connected using a crossover cable, assigned IP addresses, and tested using Simulation Mode by sending a PDU to observe packet flow.

---

## **Hardware and Software Requirements**

### **Hardware (Simulation Only)**
- A computer with Cisco Packet Tracer installed  
- Minimum **4 GB RAM** and **1 GB** free storage  

### **Software**
- Cisco Packet Tracer  
- Windows / Linux / macOS  
- Cisco NetAcad account for activation  

---

## **Procedure**

1. Open **Cisco Packet Tracer**.
2. From **End Devices**, drag **PC0** and **PC1** onto the workspace.
3. Click the **Connections** icon → select **Crossover Cable**.
4. Connect the cable:  
   - **PC0 → FastEthernet0**  
   - **PC1 → FastEthernet0**
5. Configure IP addresses:
   - **PC0:**  
     - Desktop → IP Configuration  
     - IP Address: `192.168.1.1`  
     - Subnet Mask: `255.255.255.0`
   - **PC1:**  
     - Desktop → IP Configuration  
     - IP Address: `192.168.1.2`  
     - Subnet Mask: `255.255.255.0`

---

## **Simulation Steps**

1. Click **Simulation Mode** (bottom-right corner).
2. Click **Edit Filters** and ensure **ICMP** is enabled.
3. Open **PC0 → Desktop → Command Prompt**.
4. Type:  ping 192.168.1.2
5. **Alternatively, send a PDU:**
- Click **Add Simple PDU** (envelope icon).  
- Click **PC0 → PC1**.
6. Observe packet movement in the **Event List** and workspace.
7. If the packet reaches successfully (shows **Success**), the peer-to-peer connection is working.

---

## **Result**
A peer-to-peer network was successfully simulated in Cisco Packet Tracer by directly connecting two PCs with a crossover cable, configuring IP addresses, and verifying communication using Simulation Mode using PDU and ping tests.

---

