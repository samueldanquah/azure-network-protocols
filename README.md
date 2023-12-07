<p align="center">
<img src="https://i.imgur.com/Ua7udoS.png" alt="Traffic Examination"/>
</p>

<h1>Network Security Groups (NSGs) and Inspecting Traffic Between Azure Virtual Machines</h1>
In this tutorial, we observe various network traffic to and from Azure Virtual Machines with Wireshark as well as experiment with Network Security Groups.<br />

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Various Command-Line Tools
- Various Network Protocols (SSH, RDH, DNS, HTTP/S, ICMP)
- Wireshark (Protocol Analyzer)

<h2>Operating Systems Used </h2>

- Windows 10 (21H2)
- Ubuntu Server 20.04

<h2>High-Level Steps</h2>

- Setting up Azure Virtual Machines
- Configuring Network Security Groups
- Inspecting Network Traffic with Wireshark
- Analyzing and Modifying Traffic Rules

<h2>Actions and Observations</h2>

<h3>Setting up Azure Virtual Machines:</h3>
<ul>
    <li>Deployed two VMs on Azure: one with Windows 10 and another with Ubuntu Server 20.04.</li>
    <li>Ensured both VMs were connected to the same virtual network for seamless communication.</li>
</ul>

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="VM Setup"/>
</p>
<p>
    Initial setup focused on creating a controlled environment where network traffic could be monitored.
</p>
<br />

<h3>Configuring Network Security Groups:</h3>
<ul>
    <li>Created and applied NSGs to manage the inbound and outbound traffic on both VMs.</li>
    <li>Configured specific rules to allow or deny traffic based on protocols like SSH, RDH, DNS, HTTP/S, ICMP.</li>
</ul>

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="NSG Configuration"/>
</p>
<p>
    This step was crucial in controlling how traffic flows between the VMs and external networks.
</p>
<br />

<h3>Inspecting Network Traffic with Wireshark:</h3>
<ul>
    <li>Installed Wireshark on the Windows VM to monitor and capture network traffic.</li>
    <li>Observed different types of network packets and identified patterns and anomalies.</li>
</ul>

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Wireshark Observation"/>
</p>
<p>
    Wireshark provided detailed insights into the nature and structure of the network traffic.
</p>
<br />

<h3>Analyzing and Modifying Traffic Rules:</h3>
<ul>
    <li>Based on observations in Wireshark, I adjusted NSG rules to optimize traffic flow and security.</li>
    <li>Tested the impact of these changes on network communication between the VMs.</li>
</ul>

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Traffic Rule Modification"/>
</p>
<p>
    The final step involved fine-tuning the NSG settings to ensure both security and efficiency in network communication.
</p>
<br />

<!-- Footer or additional notes -->

