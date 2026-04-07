# BRG-27-labs
# 1. Local and Cloud Infrastructure

- Download Virtualbox and Ubuntu iso

- Set up new virtual box

- Allocated 4 GB RAM, 2 CPUs, and 25 GB disk space.

<img width="1225" height="608" alt="Screenshot 2026-04-03 223755" src="https://github.com/user-attachments/assets/629da585-56bb-4631-9df3-c28eec874921" />

<img width="960" height="564" alt="image" src="https://github.com/user-attachments/assets/f3fcab17-4d7d-4ab8-a1dd-cf57fb609811" />

# 2. Linux Administration & Command Line

- Core Commands: Practiced navigation and file management using pwd, ls, cd, mkdir, and touch

<img width="960" height="564" alt="image" src="https://github.com/user-attachments/assets/e5df0592-05e6-41c0-9e21-c490273ef7cd" />

- pwd = show working directory, ls = list, cd = change directory, mkdir = make directory, touch = create file

- System Directories: Explored essential directories including /etc (configurations), /var (data), and /home (user files)

  <img width="940" height="650" alt="image" src="https://github.com/user-attachments/assets/e930b436-758e-4c19-9422-86321e09f840" />

- Manuals: Used the man command to interface with system reference manuals

<img width="940" height="650" alt="image" src="https://github.com/user-attachments/assets/9db60e6e-ee81-4529-9432-0aceb7dc8686" />

# 3. Managing and Controlling Linux Services

Background Programs: Learned that Linux relies on "Services" that run in the background

Systemctl Utility: Used systemctl to monitor and manage services

<img width="940" height="580" alt="image" src="https://github.com/user-attachments/assets/0a1400de-5e8a-4fda-93d4-863e1a2eddd0" />

Listing Units: Used systemctl list-units --type=service to observe how Ubuntu manages background processes

 Practiced checking service status with sudo systemctl status and used start or stop commands to diagnose web issues

<img width="940" height="650" alt="image" src="https://github.com/user-attachments/assets/67d43b94-3954-4732-966b-8c2f4cd831c3" />

# 4. Understanding and Applying Linux Permissions

Permission Rules: Learned that every file has specific rules for the owner, groups, and others

<img width="940" height="505" alt="image" src="https://github.com/user-attachments/assets/a305f320-e4e9-4d46-9b73-43178c8047fb" />

Long Listing: Used ls -l to view file permissions, ownership, and size

Modifying Access: Used chmod and chown to modify file access

Before

<img width="940" height="553" alt="image" src="https://github.com/user-attachments/assets/9af870ab-6171-4c0a-bb24-b5f6374692c1" />

After

<img width="940" height="647" alt="image" src="https://github.com/user-attachments/assets/08fdecb0-1640-436b-bf49-233855cb16ed" />

# 5. Searching and Navigating the Linux File System

Learning the difference between Windows searching and Linux commands like find and grep

Find Command: Used find /path -name 'filename' to enable finding a specific file location

<img width="940" height="522" alt="image" src="https://github.com/user-attachments/assets/9c3a4164-3720-4c2c-b2ba-4d4ad2051a75" />

Grep Command: Used grep to look for specific strings of text inside files

<img width="940" height="647" alt="image" src="https://github.com/user-attachments/assets/e59874a1-c877-4b76-955a-58c4ee474fcb" />

# 6. Total Cost of Ownership (TCO) in Cloud Infrastructure

Cost Comparison: Performed a TCO analysis comparing On-Premise physical hardware against AWS and Azure Cloud solutions.

<img width="940" height="269" alt="image" src="https://github.com/user-attachments/assets/9ebf5123-1b11-4c85-b26c-5e6df37c4164" />

Financial Results: Calculated a 3-year saving of $8,068 by moving to the cloud

ROI: Determined a 170% Return on Investment over a three-year period

# 7. Provisioning and Securing a Cloud VM (AWS EC2)

Cloud Transition: Transitioned from a local VM to a live AWS instance

<img width="940" height="505" alt="image" src="https://github.com/user-attachments/assets/cfb157c6-65c7-4969-9aca-de6de88b0287" />

Connection & Setup: Connected using SSH, updated the system, and installed the Apache2 web server

<img width="940" height="505" alt="image" src="https://github.com/user-attachments/assets/d87eded4-c9d7-48ec-8d8f-8d04b3b434f0" />

Manually configured rules for Port 80 (HTTP) to make the server reachable

<img width="940" height="505" alt="image" src="https://github.com/user-attachments/assets/57bcba8a-59d7-4459-b039-a6c42057ef26" />

# 8. Writing Bash Scripts and Using Regular Expressions

Automation: Created a script named lab.sh to automate system greetings

Editing: Used nano to edit index.html and other files directly on the server

<img width="940" height="505" alt="image" src="https://github.com/user-attachments/assets/227b60de-9dce-45b3-9e9a-1c96359d1486" />

Script Logic: Wrote a script using read to welcome users, including an if/else condition and a countdown for loop

<img width="940" height="505" alt="image" src="https://github.com/user-attachments/assets/763d1ea3-99ec-4d1d-befc-d5aed12e158b" />

including an if/else condition and a countdown for loop

# 9. Configuring DNS and Testing Domain Resolution

Domain Setup: Utilized DuckDNS to get a web address rather than using a raw IP

<img width="940" height="486" alt="image" src="https://github.com/user-attachments/assets/bc1b11b5-c5b9-49b5-a9c2-6856dd3ce979" />

Domain Name: Registered leroy-labs.duckdns.org

<img width="919" height="302" alt="image" src="https://github.com/user-attachments/assets/51e3301d-00cc-4894-99a3-ece9a1b33c75" />

Used nslookup to verify the domain resolves to the correct IP

# 10. Obtaining and Managing Digital Certificates with Let’s Encrypt

Secured Connection: Installed Certbot to obtain a digital certificate

<img width="940" height="505" alt="image" src="https://github.com/user-attachments/assets/710126bd-0db0-4481-aa49-4dc6177943bd" />

Troubleshooting: Encountered a "Port 80 Bind Error" because Apache was already using the port; resolved it by stopping Apache to allow Certbot to run

<img width="940" height="505" alt="image" src="https://github.com/user-attachments/assets/147a2ca3-fc15-4128-923b-4a6739ad1df4" />

Verification: Successfully enabled HTTPS, confirming the connection is secure in the browser

<img width="940" height="442" alt="image" src="https://github.com/user-attachments/assets/27b85a66-5b53-416e-ae36-1a8adb8b32f1" />

<img width="940" height="488" alt="image" src="https://github.com/user-attachments/assets/0ccaf769-99d4-41a0-944a-e54d7651fda6" />

# 11. Scripting Linux Server Functions for Automation

Learned to use Cron to make the server work 

Crontab: Used crontab -e to schedule lab.sh and logged outputs to lab_log.txt

<img width="940" height="530" alt="image" src="https://github.com/user-attachments/assets/bdb66aa8-0087-495d-9a9a-d86588596493" />

<img width="940" height="530" alt="image" src="https://github.com/user-attachments/assets/b22899db-1245-4891-b42b-8a6738e28b7b" />

# 12. Additional Server Service: MariaDB

Database Installation: Installed MariaDB-server to add a database to the environment

<img width="940" height="505" alt="image" src="https://github.com/user-attachments/assets/28a330e3-32fd-4b83-8ae4-0114e6bb447d" />

Verify MariaDB:

<img width="940" height="505" alt="image" src="https://github.com/user-attachments/assets/30ff64c8-a47e-4892-8afc-566417c850bf" />

Created a database

<img width="940" height="505" alt="image" src="https://github.com/user-attachments/assets/6b4495e6-26ba-4908-970f-f4839a84d0e6" />
