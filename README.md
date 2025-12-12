# Network Traffic Monitoring on Windows 11

## Project Summary
This project is a step-by-step tutorial that demonstrates how to monitor network traffic on a Windows 11 PC using Wireshark. It walks beginners through installation, interface selection, capturing packets, and analyzing basic protocols such as DNS, HTTP, and TCP. The project is designed as a practical hands-on walkthrough for learning foundational networking concepts.

---

## Languages Used
- No programming languages are required for this project.

---

## Environment Used
- **Windows 11**


---

## Technologies / Tools Used
- **Wireshark** — free and open-source network packet analyzer used to capture and inspect network traffic.
- **Windows 11 Command Prompt**
- **windows 11 Powershell
---

## Protocols Analyzed
- DNS
- TCP
- HTTP
- ICMP
  
---

## Demonstration Steps

### 1. Install Wireshark
Download the latest version from the official Wireshark website and run the installer with default settings.
 
<img width="490" height="381" alt="wireshark installation" src="https://github.com/user-attachments/assets/57e73204-38b3-4873-a8f8-821df91fb042" />


---

### 2. Select a Network Interface
After opening Wireshark, choose your primary network interface (Wi-Fi or Ethernet).  
This is where Wireshark will capture live packets.

<img width="929" height="531" alt="network interface" src="https://github.com/user-attachments/assets/c06a4962-3f69-4d06-b87c-d11a4e82a9b8" />



---

### 3. Start Capturing Traffic
Click **Start Capturing Packets**.  
Generate traffic by opening a browser, loading websites, or using apps.

<img width="738" height="316" alt="traffic" src="https://github.com/user-attachments/assets/27d67fe5-81df-43a7-9e09-d289a7fb8037" />


---

### 4. Analyze Collected Traffic
Use filters to break down traffic by protocol:

- `http`
- `dns`
- `tcp`
- `icmp`

Look at each packet’s source IP, destination IP, port numbers, and protocol behavior.

<img width="732" height="313" alt="tcp" src="https://github.com/user-attachments/assets/fa5d5a2f-ce7d-425c-a786-7d85759aa2e0" />


---
