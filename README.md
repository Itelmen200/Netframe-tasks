# 1. Linux
## Tasks: 
### 1.) Get web context and monitor the system:
   
   To get context from a URL, you can use the wget command to download data from the URL, for example
   ```sh
   wget https://www.google.com/
   ```
   You can also extract data using curl
   ```sh
   curl -s https://www.google.com/ | grep "<title>"
   ```
   Check CPU, memory, network, disks:

   To check the CPU use
   ```sh
   lscpu  
   ```
   or
   ```sh
   top
   ```
   To check memory use
   ```sh
   free -h
   ```

   To check the network use
   ```sh
   ifconfig
   ```
   To check the disk use
   ```sh
   df -h
   ```
   
### 2). Bash script for admin user.

   - Add user and grand the sudo access wihtout password.
   - Create file and change permissions for only sudo user access (read | write). 
   - Writing an installation program bash script.
   - Atom or other IDE.
   - Checking program availability. 
   - Use logical operators. (if, else etc)

   Add user and add to sudo group.
   
   To create a new user use:
   ```sh
   sudo adduser gleb
   ```
   
   To make it a member of the sudo group use:
   ```sh
   sudo usermod -aG sudo gleb
   ```

   Bash script installer, the script checks if the vim package is installed:
 ```ssh.bashrc
#!/bin/bash

APP="vim"

if ! command -v $APP &> /dev/null
then
        echo "$APP is not installed. Installing..."
        sudo apt-get update
        sudo apt-get install $APP
else
        echo "$APP is already installed."
fi
 ```
### Requirements for script

Save script as 'script_name.sh'

Make script executable
```sh
chmod +x script_name.sh
```
Run script
```sh
./script_name.sh
```
