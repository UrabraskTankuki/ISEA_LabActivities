# **Day1**

# Setting up Virtual machine

  - download lubuntu 24.04.2(Noble Numbat) 64bit (I downloaded from https://lubuntu.me)
  - create a virtual machine using oracle VM
  - set username and password for ubuntu account

video of how to download ubuntu: https://youtu.be/6Inw_7S2EBo

# Using Ubuntu command lines 

## CLI Familiarisation
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

## Network Configuration
network config: https://youtu.be/Cf_DxFJ2scI

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

## DNS Resolution
- nslookup google.com: Resolves google.com to its IP address using DNS

## Hardware Inspection
- lsusb: List connected USB devices
- 
  ![image](https://github.com/user-attachments/assets/41fae97c-457d-4786-801c-e668a189e787)

- lspci: Lists PCI devices
  
  ![image](https://github.com/user-attachments/assets/73e88d26-2763-4e49-8fac-ee9cb0f6f369)

- less /proc/cpuinfo: DIsplays detailed CPU information
  ![image](https://github.com/user-attachments/assets/f0a772c3-63b2-41a5-bb19-bca5978f00bc)

## Output RedirectionS
- lsusb > output_of_lsusb: saves the output of lsusb into a file
- less output_of_lsusb: view the file one page at a time
  ![image](https://github.com/user-attachments/assets/112cda99-fd01-4a36-bea7-19f136c9d137)

- cat output_of_lsusb: displays the entire file of content
  ![image](https://github.com/user-attachments/assets/e808c146-4a52-47e2-9e7a-3bd590a65b7d)

- ls -la output_of_lsusb: shows permissions of the file
  ![image](https://github.com/user-attachments/assets/3da5c02e-6bfc-41d0-ac41-6bd6742ce3ff)

- rm output_of_lsusb: deletes the file

## Software Installion and Compilation

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

## Apache Web Server
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

## Challenge 1
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

## Challenge 2
![image](https://github.com/user-attachments/assets/713c5813-4f16-46ca-8d0e-84d11965fd23)

- gedit is a graphical application and SSH does not forward GUI(X11) applications
- in this case using nano Hi_Glenn.txt would function as well
  
## Challenge 3
scp uses SSH to copy files between computers over the network
Using scp /home/glennong/Desktop/Hi_Glenn.txt glennong@127.0.0.1:/home/glennong/Desktop
![image](https://github.com/user-attachments/assets/6c65de1b-a5e0-4ef0-bde3-03d730e431c2)

## Challenge 4
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

### log into alice profile
input nano /home/sharedfile.txt to open file
![image](https://github.com/user-attachments/assets/9b1cffe0-00bb-4a3e-8fc5-61c1ec09692d)

![image](https://github.com/user-attachments/assets/f2028d12-91dc-4fe7-8667-e0947182b249)
alice can read and write the file

### log into bob profile

input cat /home/sharedfile.txt to see the text
input nano /home/sharedfile.txt to open file, it should say unwritable
![image](https://github.com/user-attachments/assets/b551a9b9-acaa-4fa3-baa8-8846e22b39cc)

![image](https://github.com/user-attachments/assets/8c34af2d-caca-4f80-a7d6-5e998f65fbbe)

### log into mallory profile
input cat /home/sharedfile.txt to see the text
![image](https://github.com/user-attachments/assets/e86cf9f6-0f92-4a7e-873d-cfd3437a8446)

## TCO (Total Cost of Ownership)

### outline
- run servers in the cloud or run your own data center locally
- Employ your own IT supoort staff or subcontracted the work
- Use Lenovo, HP, Dell AND/OR Apple as a laptop vendor

### Printer A (Budget Inkjet)
| **Cost Component**     | **Amount (AUD)** |
|------------------------|------------------|
| Printer Purchase       | $100             |
| Cartridge Cost         | $24,375          |
| Paper Cost             | $2,340           |
| Electricity Cost       | $93.60           |
| Maintenance (5 yrs)    | $100             |
| Total TCO (5 years)| $27,008.60  |

### Printer B (Business Laser)
| **Cost Component**     | **Amount (AUD)** |
|------------------------|------------------|
| Printer Purchase       | $500             |
| Cartridge Cost         | $7,800           |
| Paper Cost             | $2,340           |
| Electricity Cost       | $1,248.00        |
| Maintenance (5 yrs)    | $250             |
| Total TCO (5 years)| $12,138.00  |

### Conparison Summary Table
| **Item**                  | **Printer A (Inkjet)** | **Printer B (Laser)** |
|---------------------------|------------------------|------------------------|
| Purchase Price            | $100                  | $500                  |
| Cartridge Cost (5 yrs)    | $24,375               | $7,800                |
| Paper Cost (5 yrs)        | $2,340                | $2,340                |
| Electricity Cost (5 yrs)  | $93.60                | $1,248                |
| Maintenance (5 yrs)       | $100                  | $250                  |
| Total TCO             | $27,008.60       | $12,138.00        |

Analysis
Printers require different cost components needed to function
  - Cartridge are used to put ink on printed paper
  - paper is used as a medium for printed document
  - Electricty used is based on the how detailed the prints are from the printer
  - maintenance cost would depend on the complexity of the printer

Printer A (Inkjet) has a lower upfront cost but extremely high cartridge costs due to low page yield.

Printer B (Laser) has a higher purchase price but saves over $14,800 in TCO over 5 years thanks to efficient toner usage.

Electricity cost is higher for the laser printer, but it's still negligible compared to consumables.

Which printer is better based on TCO?
Printer B is much more cost-effective long-term.

Would your answer change for a home user who prints 5 pages/week?
Yes — for minimal printing, Printer A might be cheaper and more practical despite the high ink cost per page.

Other factors to consider?

Print quality

Speed

Noise level

Duplex (double-sided) printing

Support/Warranty

Wireless or mobile printing options

Time period where both cost the same?
You could estimate this by plotting cumulative cost over time. For this setup, Printer A quickly becomes more expensive — the break-even happens in under 1 year.

## EC2 Ubuntu Machine

name the instance Ubuntu-web-server
![image](https://github.com/user-attachments/assets/f3226082-b79d-4ea4-9b37-d741673c7ca6)

choose ubuntu server 20.04 LTS
![image](https://github.com/user-attachments/assets/f6418a08-67e1-49d4-a767-566ef141f8b3)

instance type set to t2.mirco
![image](https://github.com/user-attachments/assets/251d4d11-5bd1-4325-bd87-fed2ad8b3374)

Create a new key pair
![image](https://github.com/user-attachments/assets/45f9c302-995f-4624-a9fe-bac45bbe8ada)

set security rules as
![image](https://github.com/user-attachments/assets/db2f1019-b08a-4873-a62d-b021fe1586b9)

configure storage 
![image](https://github.com/user-attachments/assets/1a7828fa-b7b9-48e2-aee4-a2b3390a3dda)

Launch instance
![image](https://github.com/user-attachments/assets/63bd0f81-81c4-4a78-aac3-70246a6caddd)

Open terminal to ssh into terminal
enter following commands

![image](https://github.com/user-attachments/assets/d40f2a91-b3de-4708-b021-3583fac2aadb)

![image](https://github.com/user-attachments/assets/c2bef875-94a8-46dc-a0c9-a3c3ebfcfc1f)

![image](https://github.com/user-attachments/assets/ecc9c388-1347-4078-aec8-b03178ea190a)

###Install Apache
sudo apt update
sudo apt install apache2
nano /var/www/html/index.html

![image](https://github.com/user-attachments/assets/f066ab7b-95dd-400c-b153-08a460f18912)
![image](https://github.com/user-attachments/assets/2b0ff68c-258e-44d9-8ebb-6ec4d741fe15)

![image](https://github.com/user-attachments/assets/d9ddf9dc-e9d3-4ac2-adc1-ff3f307adfd3)

### Challenge 1

ping -c 4 google.com           
pings the closest region

![image](https://github.com/user-attachments/assets/5d7d5074-2d6c-4ab9-b913-68bfcc1fbdc1)

ping -c 4 amazon.co.uk
pings amazon from the uk

![image](https://github.com/user-attachments/assets/de08bd8b-9b55-4619-9e58-1694799f8f9b)

ping -c 4 facebook.com

![image](https://github.com/user-attachments/assets/86e3a0f8-885b-4279-a7e8-da2631f34365)

ping -c 4 baidu.com   
baidu is a chinese website

![image](https://github.com/user-attachments/assets/879b84c2-6cbc-489b-b4bd-e75e2acb516b)

ping -c 4 aws.amazon.com 
pings amazon in australia, cause of the EC2 is on the australian server, time is fast

![image](https://github.com/user-attachments/assets/e63462dc-de92-4145-9593-0417f2bd9df5)

### Challenge 2

scp to upload file to the EC2

![image](https://github.com/user-attachments/assets/13093f95-270c-44f6-825b-71b791bb2051)

move the file to index.html

![image](https://github.com/user-attachments/assets/0336aded-55c5-4dda-80d4-e0414e878f53)

![image](https://github.com/user-attachments/assets/f97da771-619f-4a13-bb1a-7e553a99285f)

### Challenge 3
html uses DOCTYPE as html to define the file type
every string of words are within a text type, which gives a different visual

![image](https://github.com/user-attachments/assets/6d84ac26-293e-4321-8930-41fa4d316882)
![image](https://github.com/user-attachments/assets/4ec0fad2-e072-45be-993e-eaf17ff9371e)

## BashCoding

![image](https://github.com/user-attachments/assets/8fbf44ed-4d1d-4230-93b4-9380c1165c11)
![image](https://github.com/user-attachments/assets/a9ea3b66-5dec-4f36-a643-11d45387a1c3)
![image](https://github.com/user-attachments/assets/5df68c7c-101e-4d29-84b9-e027a474873d)

![image](https://github.com/user-attachments/assets/2fe809e8-a8b8-48b8-97a3-57748e9701b5)
![image](https://github.com/user-attachments/assets/4862f23e-fd7e-4323-8f03-0bfc06949b33)
![image](https://github.com/user-attachments/assets/523dbdaf-2faf-4e58-8cbc-b66d638a1677)

copy the code 

![image](https://github.com/user-attachments/assets/bceadb90-eba4-42d1-a58c-b14ce1ead2c1)
![image](https://github.com/user-attachments/assets/d171134b-7721-420c-8cc7-2f60fb15d1c2)
![image](https://github.com/user-attachments/assets/e6fcf1a0-e49b-427a-a7cc-5641154003b0)


## DNS
sudo apt install apache2 to check if any missing files

![image](https://github.com/user-attachments/assets/59f07a8b-3951-482a-9a1c-df23714c1a2c)

Creating a domain name, i use duckDNS.org
to make a unique domain name, my website is www.asmoranomardicadaistinaculdacar.duckdns.org

![image](https://github.com/user-attachments/assets/0e07fe35-5d41-4aec-85f9-4e88b4106be7)

![image](https://github.com/user-attachments/assets/30ebd1ce-0681-4f79-99ff-8f9ff4afd789)

set the ip of the website to server IP

![image](https://github.com/user-attachments/assets/8c8def78-1ecb-4ded-a1db-1c92215121d5)
![image](https://github.com/user-attachments/assets/c660a9ed-8043-42b0-9321-69b5a4287e68)

![image](https://github.com/user-attachments/assets/d1434fea-cbc0-42b2-a417-c87cd6625aaf)

## Digital Certificates 

![image](https://github.com/user-attachments/assets/62d8219b-c081-46d5-89d8-0c88e83a9640)
![image](https://github.com/user-attachments/assets/9654d91f-ebfc-4ab5-a79a-da727eba37e4)

sudo apt update
sudo apt install snapd

![image](https://github.com/user-attachments/assets/9e91cf40-cefb-46e1-bfc4-22fe1977b034)

sudo snap install core
sudo snap refresh core

![image](https://github.com/user-attachments/assets/919353cf-d17f-48ad-b926-4f30ee0e2275)

sudo apt remove certbot
sudo snap install --classic cerbot

sudo ln -s /snap/bin/certbot /user/bin/certbot
sudo certbot --apache

![image](https://github.com/user-attachments/assets/2624b39c-d6f9-4f6d-995a-4b7f786b76a1)
![image](https://github.com/user-attachments/assets/07f361fb-da2b-4492-837c-a5bcd9a3170f)

![image](https://github.com/user-attachments/assets/1577cecf-dceb-4280-8a61-5f1b7d350c02)

## Scripting linux server functions 

create a test script
and add the following text

![image](https://github.com/user-attachments/assets/9a31933c-836e-4a26-b3e3-c4eb1b3d281b)

provide sh file privileges

![image](https://github.com/user-attachments/assets/4f89f88e-eda3-4174-adff-35d40e735b41)
![image](https://github.com/user-attachments/assets/7d2c80d0-4024-4a94-b439-e3640d557a8f)

adding variables
![image](https://github.com/user-attachments/assets/9f20d6e3-710e-4d5a-890c-17e5e07f61cb)
![image](https://github.com/user-attachments/assets/95f9c5ae-e3a8-47a4-9aff-ec49c31394eb)
![image](https://github.com/user-attachments/assets/5b282535-363b-4f84-b6f0-df58c71d14a7)

## creating backup script

![image](https://github.com/user-attachments/assets/83a3500a-8203-4fb8-8ff2-b92bd971dadd)
![image](https://github.com/user-attachments/assets/03d3a1b2-28d1-49ea-8333-927f86ff7d7d)

![image](https://github.com/user-attachments/assets/18ba3810-a2eb-4442-b24d-880de30744c3)













