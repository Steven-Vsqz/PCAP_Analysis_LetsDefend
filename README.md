<h1 align="center">PCAP Analysis on LetsDefend</h1>

The goal of this exercise is to dive into using Wireshark. LetsDefend offers a cool challenge called "PCAP Analysis" where you get a pcap (packet capture) file to review in a sandbox environment. By completing this exercise, I learned how to analyze network traffic data, understand communication patterns, spot anomalies, and detect potential security issues using Wireshark.
<br />
<br />
<strong>Wireshark</strong> is a super handy tool that lets you capture and look at network traffic in detail. For SOC analysts, it's a must-have. They use it to keep an eye on network traffic, spot any weird activity, and dig into the details when a security incident happens. Wireshark helps in finding malware, troubleshooting network issues, and providing evidence for audits or investigations. In short, it’s essential for keeping the network secure and running smoothly.
<br />
<p align="center">
<img src="https://i.imgur.com/ABECAaP.png" height="80%" width="80%" alt="Failed RDP Steps"/>
</p>

<h2>🛠️Languages and Utilities Used</h2>

![image](https://img.shields.io/badge/Wireshark-1679A7?style=for-the-badge&logo=Wireshark&logoColor=white)

- <b><a href="https://www.letsdefend.io/">LetsDefend</a>: Provides a pcap challenge in a virtual environment</b>
- <b><a href="https://www.wireshark.org/">Wireshark</a>: Popular network protocol analyzer</b>

<h2>🖥️Environments Used </h2>

- <b>Windows 10</b>

<details open>
<summary><h2>👨‍💻What was done</h2></summary>

After firing up Wireshark and opening the provided pcap file, I dug around and found a conversation with another host named “Cu713” (IP address: 192.168.235.137, MAC address: 00:0c:29:55:9d). It turns out a hidden file was uploaded to the server. On May 23, 2023, at 6:01 pm GMT, records showed an encrypted file named “file” was uploaded and placed in the uploads directory.

<h1 align="center">
Chat log: <br/>
  
![pcap_analysis_part1](https://github.com/user-attachments/assets/6debae6c-f7e8-4acf-b9c0-58cba3634c5a)

<br />
TCP steam showing upload: <br/>
<img src="https://i.imgur.com/ggOsKAh.png" height="80%" width="80%" alt="Failed RDP Steps"/>
<br />
</h1>

</details>
<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>
