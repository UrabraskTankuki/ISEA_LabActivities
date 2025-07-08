![image](https://github.com/user-attachments/assets/91c58243-7aec-4e12-90d0-ade7a0f15766)![image](https://github.com/user-attachments/assets/67c8b581-3048-4e6a-a287-eaa65d84060a)# BridgingLabLinux

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

- nslookup google.com
- lsusb
- lspci
- less /proc/cpuinfo


  







   

