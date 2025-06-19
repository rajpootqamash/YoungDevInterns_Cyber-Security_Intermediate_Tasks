# 🌐 Task 3: Analyze Network Traffic Using Wireshark

## 🎯 Purpose

The purpose of this task is to learn how to capture, monitor, and analyze live network traffic using **Wireshark**, one of the most powerful packet analysis tools available. Understanding traffic patterns, protocols, and anomalies helps in identifying potential threats or suspicious activity on a network.

## 🧰 Tools Used

- **Wireshark** – A GUI-based packet sniffer and protocol analyzer.
- **Kali Linux / Windows / macOS** – Wireshark is cross-platform.
- **Network Adapter** – To capture live traffic on the connected interface.


## 🪜 Step-by-Step Procedure

### ✅ Step 1: Install Wireshark (if not installed)
If you're using Kali Linux, Wireshark is usually pre-installed. If not:

          sudo apt update
          sudo apt install wireshark
![15](https://github.com/user-attachments/assets/f814e3a4-a377-4002-a194-e60ffb114650)

### ✅ Step 2: Launch Wireshark with Root/Sudo
Run Wireshark with elevated privileges to capture packets:

            sudo wireshark

### ✅ Step 3: Select the Active Network Interface
- Choose the interface with live traffic (e.g., eth0, wlan0, or en0).
- Double-click the interface to begin capturing packets.
            
![16](https://github.com/user-attachments/assets/3cf9c1c0-3147-4d93-a798-9a59ab7e7945)

### ✅ Step 4: Start Capturing Packets
Once the interface is selected:

- Click the blue shark fin icon or "Start Capturing" button.
- Let Wireshark run while you browse the internet or run some network activity (e.g., ping google.com or open websites).
  
  ![17](https://github.com/user-attachments/assets/cf714dce-d1c4-4966-934d-bcdf45802186)

### ✅ Step 5: Apply Display Filters
To analyze specific types of traffic, use filters like:

- http – show only HTTP traffic
- tcp – show TCP packets
- dns – show DNS queries and responses
- ip.addr == x.x.x.x – filter traffic by IP address

 ### ✅ Step 6: Analyze Individual Packets
Click on a packet to view:

- Source and destination IP
- Protocol (TCP, UDP, HTTP, etc.)
- Packet length and info
- Detailed headers and data in the lower pane

### ✅ Step 7: Stop and Save the Capture
After collecting sufficient data:
- Click the red Stop button.
  
![18](https://github.com/user-attachments/assets/8896a4c6-6459-4d45-8796-a375c6392d8d)

![19](https://github.com/user-attachments/assets/f7a5a25e-adc4-4c26-9f51-fe2fc10492e6)

![20](https://github.com/user-attachments/assets/4e9bb96c-d620-4616-97c9-ecba9a5ec338)

![21](https://github.com/user-attachments/assets/4dab64c6-427f-41c7-8d57-26b3b61cecf2)

## 🔍 What to Observe
- Number of packets captured
- Protocols in use (TCP, UDP, HTTP, DNS, etc.)
- Destination IPs of traffic
- Suspicious or unexpected connections
- Whether any credentials or sensitive info are visible in plaintext (HTTP)

## 📌 Important Notes
- Use Wireshark only on networks you own or have permission to analyze.
- Avoid running packet captures on public Wi-Fi or unauthorized networks.
- Sensitive information (e.g., passwords) might be visible in unencrypted traffic (e.g., HTTP).

## ✅ Conclusion:

In this task, you used Wireshark to capture and analyze network traffic. You learned how to select an interface, apply filters, inspect packets, and save your captures. This skill is essential for network security analysts, ethical hackers, and system admins to detect intrusions, analyze suspicious behavior, or troubleshoot network issues.
