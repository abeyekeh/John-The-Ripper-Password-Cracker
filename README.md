# Building and understanding John the Ripper password cracker on Kali for cyber security practice

# Step One
- I installed john is install on my kali system, sometime john is installed, check the version to confrim or install/update ther current version by using the command the following command 
- sudo apt-get install john

# Step Two
- I created a simple file with an MD5 hash to store the password for john the Ripper to crack
- echo -n "password" | md5sum | awk '{print $1}' > thepasswordyouwant.txt
- than run a command to get john cracking, i used
- john --format=Raw-MD5 thepasswordtxtfileyoucreated.txt
- this command find the hash for password and printed it, the password can only be hash once
- cat ~/.john/john.pot
- 