# Netframe-tasks
1. Linux
   1). Get context from URL.
   To get context from a URL, you can use the wget command to download data from the URL, for example:
   wget https://www.google.com/

   You can also extract data using curl:
   curl -s https://www.google.com/ | grep "<title>"

   2). Check CPU, memory, network, disks:
   To check the CPU use:
   lscpu or top

   To check memory use:
   free -h

   To check the network use:
   ifconfig

   To check the disk use:
   df -h

   3). Add user and add to sudo group.
   To create a new user use:
   sudo adduser gleb

   To make it a member of the sudo group use:
   sudo usermod -aG sudo gleb

   4). 
