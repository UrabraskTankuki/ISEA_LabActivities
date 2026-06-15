

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
video of working demo: https://youtu.be/3wpwqoxIkk8

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

## Reflection
https://youtu.be/IyQL6bjEDuY










