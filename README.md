# Document-Network-Intrusion-and-Sniffing 
## Project Overview
In this project I will be demonstrating a Network Attack with my home wifi; the intruder will find my network, gain access, scan my local devices, and start tapping the outbound traffic of a target device through ARP Poisoning.

## 1. setup
For this project I will be using Parrot OS combined with a network adapter and the tools below.

•	airodump-ng  
•	airodump-ng  
•	ettercap  
•	wireshark  

## 2. Reconnaissance

• Set the adapter in monitor mode and use airodump-ng to monitor networks within range. Target a network and get their BSSID and operating channel.    
• Use airodump to associate clients with a given access point, get the client MAC address, and set a dumpfile to start collecting their network traffic/comms.   

<img width="3840" height="2036" alt="1" src="https://github.com/user-attachments/assets/649fc33d-e460-4146-af6c-a89ad5b08a12" />

<img width="3840" height="2095" alt="3" src="https://github.com/user-attachments/assets/982d3d6e-cbe3-4eb0-8c6e-76a7134fdf92" />

<img width="3779" height="766" alt="4" src="https://github.com/user-attachments/assets/d8472f8b-f22f-4aa6-b03b-f8c55417c061" />


## 3. De-authentication Attack
• use aireplay-ng to target a client, and send deauthentication packets to disassociate them with the AP, knocking them off the network.   


## 4. Capture EAPOL Handshake
• As the device reconnects to their trusted network, airodump will capture the WPA handshake between the client and the AP; you can verify all parts of the EAPOL message in Wireshark.

<img width="3840" height="2025" alt="handshake" src="https://github.com/user-attachments/assets/eb42bff4-face-49e5-83d1-a60168087ef0" />

## EPOL Handshak in Wireshark
<img width="3840" height="1953" alt="Wireshark eapol" src="https://github.com/user-attachments/assets/bbe9b70d-793f-420f-ae93-2556635a7f4a" />




## Pakcet Analysis 
• Wireshark used for detailed packet capture and packet analysis.  


<img width="3840" height="1911" alt="Wireshark packet" src="https://github.com/user-attachments/assets/e4d6de2a-271f-4aee-ab02-6b004130436a" />







