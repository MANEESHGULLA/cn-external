# LAN Simulation Using Three PCs and a Switch in Cisco Packet Tracer

## **Aim**
To simulate a local area network (LAN) by connecting three PCs to a single switch using straight-through cables and verify communication using Simulation Mode in Cisco Packet Tracer.

---

## **Description**
A LAN allows multiple computers to communicate through a switching device. In this simulation, three PCs are connected to a switch using straight-through cables. After assigning IP addresses, connectivity is tested using Simulation Mode and by sending PDU packets.

---

## **Hardware and Software Requirements**

### **Hardware (Simulation Only)**
- Computer with Cisco Packet Tracer installed  
- Minimum **4 GB RAM**, **1 GB** free storage  

### **Software**
- Cisco Packet Tracer  
- Windows / Linux / macOS  
- Cisco NetAcad account for activation  

---

## **Procedure**

### **Network Setup**

1. Open **Cisco Packet Tracer**.
2. From **End Devices**, drag **PC0**, **PC1**, and **PC2** onto the workspace.
3. From **Switches**, drag a **2960 switch** into the workspace.
4. Click **Connections** → select **Straight-Through Cable**.
5. Connect cables as follows:  
   - **PC0 → Switch FastEthernet0/1**  
   - **PC1 → Switch FastEthernet0/2**  
   - **PC2 → Switch FastEthernet0/3**

---

### **Assign IP Addresses**

- **PC0**  
  - IP Address: `192.168.1.1`  
  - Subnet Mask: `255.255.255.0`

- **PC1**  
  - IP Address: `192.168.1.2`  
  - Subnet Mask: `255.255.255.0`

- **PC2**  
  - IP Address: `192.168.1.3`  
  - Subnet Mask: `255.255.255.0`

---

## **Simulation Steps**

1. Click **Simulation Mode** (bottom right).
2. Click **Edit Filters** and ensure **ICMP** is enabled.
3. Perform ping tests:

   On **PC0** → Command Prompt
   ping 192.168.1.2
   ping 192.168.1.3

4. **Send PDU (Simple Packet):**
- Click **Add Simple PDU** (envelope icon)
- Click **PC0 → PC1**
- Repeat **PC0 → PC2**
5. Observe packet movement and the **Event List**.  
Successful status indicates correct communication.

---

## **Result**
A LAN with three PCs connected to a switch was successfully simulated in Cisco Packet Tracer using straight-through cables. All PCs communicated with each other after proper IP configuration, verified through Simulation Mode using PDU and ping tests.

---

