## Day1

## Setting up Virtual machine

  - download lubuntu 24.04.2(Noble Numbat) 64bit (I downloaded from https://lubuntu.me)
  - create a virtual machine using oracle VM
  - set username and password for ubuntu account

## Using Ubuntu command lines 

 - ubuntu commands refer to directories in the system
 - each command interacts with the directory in different ways
 - this are a list of commands that are generally used
   
   ![image](https://github.com/user-attachments/assets/852773c5-985a-4602-9f26-d3802a8d4b6c)
   ![image](https://github.com/user-attachments/assets/53853b1f-22a9-4b27-9eb8-d4215bfea375)

 - manual commands are commands that display information and use of commands
   ![image](https://github.com/user-attachments/assets/17afba1a-fc77-4d15-82bc-b4921b98e125)
   ![image](https://github.com/user-attachments/assets/10441f5f-72c0-4570-9de8-08a1b030b6d5)
   ![image](https://github.com/user-attachments/assets/27367be2-e652-4206-a55f-944465c288f9)
   
## Using Ubuntu command lines 

### CLI Familiarisation
- ps -e: lists all current running processes
  ![image](https://github.com/user-attachments/assets/bca7ee8e-2776-4262-9438-54f0359256bf)

- top: Shows realtime CPU process usage and memory
  ![image](https://github.com/user-attachments/assets/74eac91a-f4da-445d-9ff1-98730dcba4c3)

- ls: List files and directories in current location
  ![image](https://github.com/user-attachments/assets/026b2e47-a5b9-4e3a-a4c3-d13ac28806cd)

- ls -la: List all files with detailed info
  ![image](https://github.com/user-attachments/assets/2fd7e0e4-68c3-40f3-955a-3e3c84506e35)

- touch testfile: touch creates a file, and testfile is the name of the file
- gedit testfile: opens testfile in a graphical text editor (requires download using sudo apt install gedit)
  ![image](https://github.com/user-attachments/assets/9e705594-0f7e-400e-8fc3-c016812308a4)

- featherpad testfile: opens testfile in a graphical text editor
  ![image](https://github.com/user-attachments/assets/fcdceee8-b548-4b7c-9d7c-cf8e8480c185)
  
- nano testfile: opens a testfile in the terminal text editor (ctrl + x to exit out of text editor)
  ![image](https://github.com/user-attachments/assets/42b2a3b7-3158-4c59-b8de-12b49463a016)

- cat testfile: display contents of the test file
  ![image](https://github.com/user-attachments/assets/e63780d3-31d8-4878-80c5-910c9c4c9aea)

- less testfile: scrollable view of the file contents
  ![image](https://github.com/user-attachments/assets/5d576829-ef9a-4721-8a65-a17bda77de4f)
  
- cp testfile testfile2: copy contents in testfile into testfile
  ![image](https://github.com/user-attachments/assets/02dd45c9-0ef9-4443-9c17-10be64514c71)

- mv testfile2 testfile3: moves all contents in testfile2 into testfile3
  ![image](https://github.com/user-attachments/assets/908fdb1f-4138-4b10-8483-95a71de2af3e)

- uname -a: shows detailed system information
  ![image](https://github.com/user-attachments/assets/f26d43bd-64f2-4ef3-b2b0-d394a8bf8fde)

- lsb_release -a: display Ubuntu version and release details
  
  ![image](https://github.com/user-attachments/assets/5652a925-22b3-4bdd-9508-e1780d2e568b)

- hostnamectl: show host settings and allows ways to modify hostname and OS details
  ![image](https://github.com/user-attachments/assets/6d2694df-89a2-4e10-a438-f4465f5aade3)

- ls -alt: list all files, sorted by recently modified and newest to last
  ![image](https://github.com/user-attachments/assets/e206e245-bf6c-4000-b11c-a97edcae16c0)

### Super User
- whoami: prints current username
  
  ![image](https://github.com/user-attachments/assets/69d01435-749f-4fcc-98f8-e3415a694974)S

- adduser testuser: creates a new user which requires "sudo" as root privileges
  ![image](https://github.com/user-attachments/assets/6cd76ada-153a-40d8-bc2c-97de661859df)

- sudo whoami: Runs whoami as root, to show the level of privileges
  
  ![image](https://github.com/user-attachments/assets/b1f8f6d3-853b-4a13-be8b-77cf94b08e2b)

- sudo adduser testuser: creates a new user
  ![image](https://github.com/user-attachments/assets/3219f5fa-dd22-4817-92c0-22e6e126963a)

### Netowrk Configuration
- ip a: disaplays network interface and IP addresses
  ![image](https://github.com/user-attachments/assets/1c23fd22-2ec5-463f-9494-c9cd315710f7)

- ping 8.8.8.8: pings google.com every second and stops only after ctrl + Z
  ![image](https://github.com/user-attachments/assets/457687e4-0969-42e1-8516-a94e8b21d221)
  
- less /etc/hosts: shows local files
  ![image](https://github.com/user-attachments/assets/79f1001c-7899-4ef8-96c4-7d82e65b99e3)

- sudo nano /etc/hosts: edits the hosts file with root permission
  ![image](https://github.com/user-attachments/assets/bde5a843-21aa-4025-878e-26cf7ab45dff)
  
- ping localhost: pings localhost's ip
  
  ![image](https://github.com/user-attachments/assets/47b51bd6-aa2e-4ff3-ae4a-202cbf82420f)

- ping testServer: testServer is an aliases, ping will ping the ip of the testServer
  ![image](https://github.com/user-attachments/assets/ae0fbc1b-0ce9-4c57-a964-e3bb415e19d8)
  ![image](https://github.com/user-attachments/assets/7fe742a9-b7bd-4d04-be09-be745a1c13e3)

### DNS Resolution
- nslookup google.com: Resolves google.com to its IP address using DNS

### Hardware Inspection
- lsusb: List connected USB devices
- 
  ![image](https://github.com/user-attachments/assets/41fae97c-457d-4786-801c-e668a189e787)

- lspci: Lists PCI devices
  
  ![image](https://github.com/user-attachments/assets/73e88d26-2763-4e49-8fac-ee9cb0f6f369)

- less /proc/cpuinfo: DIsplays detailed CPU information
  ![image](https://github.com/user-attachments/assets/f0a772c3-63b2-41a5-bb19-bca5978f00bc)

### Output RedirectionS
- lsusb > output_of_lsusb: saves the output of lsusb into a file
- less output_of_lsusb: view the file one page at a time
  ![image](https://github.com/user-attachments/assets/112cda99-fd01-4a36-bea7-19f136c9d137)

- cat output_of_lsusb: displays the entire file of content
  ![image](https://github.com/user-attachments/assets/e808c146-4a52-47e2-9e7a-3bd590a65b7d)

- ls -la output_of_lsusb: shows permissions of the file
  ![image](https://github.com/user-attachments/assets/3da5c02e-6bfc-41d0-ac41-6bd6742ce3ff)

- rm output_of_lsusb: deletes the file

### Software Installion and Compilation

- sudo apt install whois : installs the whois tool from package manager
- sudoo apt search vl: searches for VLC package availability
  ![image](https://github.com/user-attachments/assets/f75ad39f-7560-498b-a416-e4d072aba377)

- sudo apt install vlc: install VLC player
- sudo apt update: Updates the list of available packages
- sudo apt upgrade: Installs the latest versions of installed packages
  ![image](https://github.com/user-attachments/assets/d16739fb-3fb8-4da8-99b7-cd46d3ea8f4c)

- sudo apt install build-essentials: installs tools for compiling
- gcc hello_world.c -o hello_world_executable: Compiles C file into an executable
- chmod 777 hello_world_Executable: Grants full permissions to all users

###Apache Web Server
- sudo apt update: updates any outdated softwares
- sudo apt install apache2: installs apache web server
- sudo apt install nmap: installs nmap network scanning tool
- sudo apt install openssh-server
- ip a: shows info about ip address
  ![image](https://github.com/user-attachments/assets/85904fe5-94dc-4450-8c2f-9d99b2746574)

- nano /var/www/html/index.html: opens apache web page
  ![image](https://github.com/user-attachments/assets/48691df7-3beb-484a-a461-be80265f81ef)

  
- sudo nano /var/www/html/index.html: grants permission to edit the file

- sudo ufw status verbose: used to change the status of the UFW(Uncomplicated Firewall)
- sudo ufw enable: enables firewall
  
  ![image](https://github.com/user-attachments/assets/7911ad15-5b70-4e3d-976c-0669788d02dd)

### Challenge 1
SSH of my own machine and file with "Hi_Glenn"

Step 1: install all software require to start SSH server
  - sudo apt update 
  - sudo apt install openssh-server
    ![image](https://github.com/user-attachments/assets/873d9bd2-2868-4f45-aba8-bffb98087018)

  - sudo systemctl enable ssh
  - sudo systemctl start ssh

    ![image](https://github.com/user-attachments/assets/154f3e6d-dd0c-4425-a045-62949a9e7fbe)

Step 2: Find IP Address
  - ip a to find ip
    
    ![image](https://github.com/user-attachments/assets/220fabdb-0443-48ca-8ef7-ff95f889b7cc)
    
  - ip is 127.0.0.1/8
    
Step 3: SSH using default user
  - ssh glennong@localhost
    ![image](https://github.com/user-attachments/assets/2a3da3ee-c562-469e-a958-aefe392f19a8)

Step 4: Create file to desktop
  - cd ~/Desktop to go to desktop directory
  - echo "Hi_Glenn" > Hi_Glenn.txt
  - exitS
    ![image](https://github.com/user-attachments/assets/b9dd4e8e-b5e6-4cad-a90d-ef9bd5612d71)

### Challenge 2
![image](https://github.com/user-attachments/assets/713c5813-4f16-46ca-8d0e-84d11965fd23)

- gedit is a graphical application and SSH does not forward GUI(X11) applications
- in this case using nano Hi_Glenn.txt would function as well
  
### Challenge 3
scp uses SSH to copy files between computers over the network
Using scp /home/glennong/Desktop/Hi_Glenn.txt glennong@127.0.0.1:/home/glennong/Desktop
![image](https://github.com/user-attachments/assets/6c65de1b-a5e0-4ef0-bde3-03d730e431c2)

### Challenge 4
download the file as plain text UTF-8 
as wget filename.txt
![image](https://github.com/user-attachments/assets/c1bcd0e0-f341-41f8-913c-28bd13f68b70)
move all the text files to gutenberg_top10 file

compress the folder using tar.gz
![image](https://github.com/user-attachments/assets/66ef4358-64cf-4fae-bf08-2104dba43cf3)

use scp to send the files to Desktop
![image](https://github.com/user-attachments/assets/ca17bdfd-eaed-4d71-8ed2-0f9d19367118)

## linux Permissions
Create 3 new user Alice, Bob and Mallory

create a file sharedfile.txt and make alice an owner

![image](https://github.com/user-attachments/assets/60ed83ff-6961-49d8-8d3a-4b72706bf42c)


Create a group add alice and bob to the group as projectgroup

![image](https://github.com/user-attachments/assets/32255bfa-8329-406c-a30a-16e8fc727ea0)

assign projectgroup the file sharedfile.txt
grant bob permission for reading but no writing

![image](https://github.com/user-attachments/assets/08118ab7-01d0-4eff-a5c6-752e7b02f39b)

#### log into alice profile
input nano /home/sharedfile.txt to open file
![image](https://github.com/user-attachments/assets/9b1cffe0-00bb-4a3e-8fc5-61c1ec09692d)

![image](https://github.com/user-attachments/assets/f2028d12-91dc-4fe7-8667-e0947182b249)
alice can read and write the file

#### log into bob profile

input cat /home/sharedfile.txt to see the text
input nano /home/sharedfile.txt to open file, it should say unwritable
![image](https://github.com/user-attachments/assets/b551a9b9-acaa-4fa3-baa8-8846e22b39cc)

![image](https://github.com/user-attachments/assets/8c34af2d-caca-4f80-a7d6-5e998f65fbbe)

#### log into mallory profile
input cat /home/sharedfile.txt to see the text
![image](https://github.com/user-attachments/assets/e86cf9f6-0f92-4a7e-873d-cfd3437a8446)







   

