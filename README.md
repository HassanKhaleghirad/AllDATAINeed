# AllDATAINeed
imporatant Command 

https://askubuntu.com/questions/1039233/no-wired-connection-wired-unmanaged-ubuntu-18-04

I had exactly the same problem, but then tracked down the following solution (via this article).

Add a missing config file with

 sudo touch /etc/NetworkManager/conf.d/10-globally-managed-devices.conf
Edit /etc/NetworkManager/NetworkManager.conf (needs to be done with sudo) changing the line managed=false to read managed=true

Restart network manager with

 sudo service network-manager restart


.h library add to c program in terminal 
gcc example_sign.c -o example_sign -I/home/hassan/Documents/sinafile/codes     ->/openssl/digest.h
