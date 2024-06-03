## 1. Linux
# Tasks: 
1.) Get web context and monitor the system:
   
   To get context from a URL, you can use the wget command to download data from the URL, for example:
   ```sh
   wget https://www.google.com/
   ```
   You can also extract data using curl:
   ```sh
   curl -s https://www.google.com/ | grep "<title>"
   ```
   Check CPU, memory, network, disks:

   To check the CPU use:
   ```sh
   lscpu  
   ```
   or
   ```sh
   top
   ```
   To check memory use:
   ```sh
   free -h
   ```

   To check the network use:
   ```sh
   ifconfig
   ```
   To check the disk use:
   ```sh
   df -h
   ```
   
2). Bash script for admin user.

   - Add user and grand the sudo access wihtout password.
   - Create file and change permissions for only sudo user access (read | write). 
   - Writing an installation program bash script.
   - Atom or other IDE.
   - Checking program availability. 
   - Use logical operators. (if, else etc)

