# OPNsense-Suricata
Configure Suricata IDS/IPS for OPNsense
GOAL: Enable Intrusion detection and intrusion prevention services to monitor your network for sybsecurity threats and prevent unauthorized access.

This walk through assumes you have a functioning OPNsense firewall device configured and functioning. You will need root level access to complete the following steps.

Step 1. Installing the Suricata Plugin- Navigate to “System -> Firmware -> Plugins” and install the two intrusion detection open plugins. It is possible that Instrusion detection might already be installed on your version of OPNsense. To check, navigate to services and choose Intrustion Detection. There will be a checkbox to also enable IDS, a second checkbox to enable IPS mode (please also check promiscious mode if you intend to use VLAN). In my installation, I chose to use Suricata to monitor WAN traffic(choose WAN interface), and later I setup ZENARMOR to monitor LAN traffic. 
![image](https://github.com/CyberDanMan/OPNsense-Suricata/assets/164780036/23bef420-4d04-490f-bc58-748ec22dacb2)
