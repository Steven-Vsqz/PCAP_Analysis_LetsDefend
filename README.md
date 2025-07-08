# 🕵️‍♂️ PCAP Analysis on LetsDefend
<p align="center">
  <img src="https://i.imgur.com/ABECAaP.png" width="80%" alt="PCAP Analysis Screenshot" />
</p>

This project demonstrates network packet analysis using **Wireshark** in a simulated SOC challenge hosted on [LetsDefend.io](https://www.letsdefend.io/). By working through the **PCAP Analysis** lab, I gained hands-on experience identifying suspicious communication patterns, isolating malicious activity, and uncovering file transfers from raw traffic captures.

---

## 🛠️ Tools & Technologies Used

<div align="center">

![Wireshark](https://img.shields.io/badge/Wireshark-1679A7?style=for-the-badge&logo=Wireshark&logoColor=white)

</div>

- [LetsDefend.io](https://www.letsdefend.io/) — Virtual SOC training platform offering real-world scenarios  
- [Wireshark](https://www.wireshark.org/) — Industry-standard network protocol analyzer for traffic inspection

---

## 💻 Environment

- **Windows 10** (host system)
- **Sandboxed analysis environment** provided by LetsDefend

---

<details open>
<summary><h2>🔍 What I Did</h2></summary>

Using Wireshark, I loaded the provided `.pcap` file and began investigating an unusual session. During the inspection, I discovered:

- A suspicious conversation between the host and a machine identified as `Cu713`  
  - **IP:** `192.168.235.137`  
  - **MAC:** `00:0c:29:55:9d`
- At **6:01 PM GMT on May 23, 2023**, an **encrypted file** named `file` was **uploaded** to a server and stored in the `/uploads` directory

The TCP stream clearly showed file transfer activity indicative of data exfiltration or covert communication.

---

### 🗂️ Evidence Screenshots

#### 📁 Chat Log (Decoded)
<p align="center">
  <img src="https://github.com/user-attachments/assets/6debae6c-f7e8-4acf-b9c0-58cba3634c5a" width="75%" alt="Chat Log Screenshot" />
</p>

#### 📤 TCP Stream Showing File Upload
<p align="center">
  <img src="https://i.imgur.com/ggOsKAh.png" width="80%" alt="TCP Upload Screenshot" />
</p>

</details>

---

## 🎯 Key Skills Demonstrated

- 📡 Deep packet inspection with Wireshark
- 🔎 Identifying lateral movement and suspicious file uploads
- 📁 Analyzing TCP streams and extracting indicators of compromise (IOCs)
- 💬 Interpreting raw protocol data to build attack timelines
- 🧠 SOC-aligned analytical thinking

---

## 🚀 Next Steps

- Practice dissecting HTTP, DNS, and SMB traffic for threat hunting  
- Automate packet filtering using **tshark** or scripting  
- Apply learned techniques in real-world CTFs or other LetsDefend labs

---

<p align="center"><i>✅ This project strengthens my SOC analysis and threat detection skills, showing my readiness for an entry-level cybersecurity role.</i></p>
