1.)Crack the password of attached file using John the Ripper (just like 
Fcrackzip):

Step 1:get the password hash 
To get the password hash to be cracked, we need to enter the 
command: 
$zip2john GradedLab1.zip 

Step 2:put the password hash in a text file 
Type the following command : 
$zip2john GradedLab1.zip > hash121.txt 

Followed by: 
$John hash.txt 

The command above initiates John the Ripper, a proficient password cracking 
tool.   

The txt file contains the message:

<img width="812" height="251" alt="image" src="https://github.com/user-attachments/assets/59e988aa-e25a-4ab5-8a5d-9fe41e1a2350" />
