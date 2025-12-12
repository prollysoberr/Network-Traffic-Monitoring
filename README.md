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
- **windows 11 Powershell**
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

---

Run the following in Command Prompt

```ping google.com```

This produces ICMP Echo Request and Echo Reply packets.  
<img width="553" height="340" alt="cmd prompt" src="https://github.com/user-attachments/assets/d53a57f4-831e-4f98-ae3a-7e8306d96c04" />

Go back to Wireshark and Apply filter: `icmp`

<img width="739" height="268" alt="icmp" src="https://github.com/user-attachments/assets/c186e55b-78e2-4760-b11d-a16e1891b846" />

---

Open any website in your browser (e.g., `example.com`).  
Your PC will send DNS queries automatically.

Go back to Wireshark and Apply filter `dns`	

---

Run the following command in Powershell

```Test-NetConnection -ComputerName google.com -Port 80```

Go back to Wireshark and Apply filter:`tcp`

---

Visit a non-HTTPS site such as ```neverssl.com```
This produces readable HTTP traffic

Go back to Wireshark and Apply filter:`http`

---

Look at each packet’s source IP, destination IP, port numbers, and protocol behavior.

<img width="732" height="313" alt="tcp" src="https://github.com/user-attachments/assets/fa5d5a2f-ce7d-425c-a786-7d85759aa2e0" />


---
