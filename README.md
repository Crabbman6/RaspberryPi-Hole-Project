# RaspberryPi-Hole-Project
Raspberry Pi Hole Setup Project


First I have installed Raspberry Pi Imager to put Raspberry Pi Os Lite 64 Bit onto my SD Card. This is the operating system the Pi will run on. 

<img width="1004" height="641" alt="image" src="https://github.com/user-attachments/assets/b38a972d-4a89-49f3-b581-01bb64fdcefc" />

<img width="1006" height="639" alt="image" src="https://github.com/user-attachments/assets/5b3f83e1-a474-4de8-89ac-3ad14b217626" />


Here I'm connecting to the Pi over SSH now it has been plugged in. The hostname would not resolve so I used the IP address assigned instead. This will be changed to a different static value in the router settings. 

<img width="1103" height="604" alt="image" src="https://github.com/user-attachments/assets/0fab453f-8c69-47f7-8cbb-0aad2b453dd3" />

Updating the OS before proceeding. 

<img width="1105" height="620" alt="image" src="https://github.com/user-attachments/assets/bd7a1c3b-85a5-4af8-9349-aa34eb964f35" />


<img width="1110" height="611" alt="image" src="https://github.com/user-attachments/assets/b655c97a-5e11-46eb-8bf6-847662b52489" />

Assigning the Pi a reserved private IP address 

<img width="2223" height="192" alt="image" src="https://github.com/user-attachments/assets/14ac9996-d199-495d-9dbc-a2f8f849d8e3" />

Using Quad9 DNS Stream Provider as it focuses on privacy and security.

<img width="1078" height="615" alt="image" src="https://github.com/user-attachments/assets/1106608d-e6f4-4103-b6c7-dcef4e8e34dc" />

PiHole software has been installed on the OS. 

<img width="1103" height="620" alt="image" src="https://github.com/user-attachments/assets/bc3026a8-6df4-49f9-982c-b1e401945259" />

PiHole Admin Dashboard

<img width="1239" height="1014" alt="image" src="https://github.com/user-attachments/assets/25502ef6-3e69-4db6-a4db-dc1334d859a2" />

Blocklists HaGeZi Pro	for adblock and tracking 

aGeZi TIF Mini	for threat intelligence

<img width="974" height="436" alt="image" src="https://github.com/user-attachments/assets/a2f9ccc9-4d62-46c0-b878-5f15a6681cd1" />

# Making the Pi work for the entire network

Now that I have tested the PiHole works by setting my DNS server per device, I'm going to make the Pi the DHCP server and also change this within the router settings. 


Saves name of network profile and saves into a variable then saves the settings to that profile. Sets the Pi to use a static address instead of requesting one via DHCP, then sets the static IP. Quad9 is used as the DNS resolver, then reactivates the connection to apply changes.
<img width="1105" height="620" alt="image" src="https://github.com/user-attachments/assets/27588aac-ee08-4635-b8ea-ae6fd46f5ae5" />
