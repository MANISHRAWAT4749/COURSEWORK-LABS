1.)Crack the password of attached file using John the Ripper (just like 
Fcrackzip):

Step 1:get the password hash 
To get the password hash to be cracked, we need to enter the 
command: 
$zip2john GradedLab1.zip 

Step 2:put the password hash in a text file 


Type the following command : 
$zip2john GradedLab1.zip > hash121.txt 
<img width="940" height="156" alt="image" src="https://github.com/user-attachments/assets/77e8ef8b-67c9-4217-8df8-06ece57d0dd1" />


Followed by: 
$John hash.txt 

The command above initiates John the Ripper, a proficient password cracking 
tool.  
<img width="940" height="635" alt="image" src="https://github.com/user-attachments/assets/3c813a22-ba0a-4602-87c3-a506e2fe2770" />



The txt file contains the message:

<img width="812" height="251" alt="image" src="https://github.com/user-attachments/assets/59e988aa-e25a-4ab5-8a5d-9fe41e1a2350" />
