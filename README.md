# INSA-notes
week1
Downloading Vbox and Kali Linux

Linux
VirtualBox is a virtualization software developed by  that allows users to run multiple operating systems on a single computer. It creates virtual machines where different systems can be installed and tested safely without affecting the main system.
Kali Linux is a Debian-based Linux distribution developed by . It is widely used for cybersecurity, penetration testing, and ethical hacking. Kali Linux comes pre-installed with many security tools used for network analysis, vulnerability testing, and digital forensics.
VirtualBox is commonly used to run Kali Linux on a PC, making it easy for learners and professionals to practice cybersecurity in a safe and controlled environment.
week1 day2
Kali Linux is a Linux-based Operating System (OS) designed for:
Ethical hacking
Penetration testing (Pentesting)
Cybersecurity learning
It comes with built-in tools used by:
🔴 Red Team (attackers)
🔵 Blue Team (defenders)
It is mainly used through the Terminal (CLI – Command Line Interface)
💻 Kali Linux Terminal Commands
Bash
pwd → Print Working Directory

ls → List files and folders

ls -a → List all files (including hidden)

cd folder_name → Enter directory

cd .. → Go back one directory

mkdir folder_name → Create folder

mkdir -p a/b/c → Create nested folders

touch file.txt → Create empty file

rm file.txt → Delete file

rm -r folder_name → Delete folder

cp file1 file2 → Copy file

mv file1 file2 → Move or rename file

cat file.txt → View file content

echo "text" > file.txt → Write into file

chmod 755 file.txt → Change permissions

clear → Clear terminal

history → Show previous commands
🔐 Permissions (4-2-1 Rule)
Bash
4 → Read (r)

2 → Write (w)

1 → Execute (x)

Example:
chmod 755 file.txt

Owner → 7 (rwx)

Others → 5 (r-x)
 Blue Team vs  Red Team
 Red Team (Attackers)
Simulate hackers to find system weaknesses
Goal: Break into the system (ethically)
Bash
/etc/shadow → password hashes

/tmp → hide scripts or malware
What they do:
Exploit vulnerabilities
Crack passwords
Gain access
🔵 Blue Team (Defenders)
Protect systems and detect attacks
Goal: Secure and monitor systems
Bash
/var/log → system logs

/etc → configuration files
What they do:
Monitor activity
Detect threats
Defend systems


Week2 day1

Linux User Management 
to give permission to users,
root user:the main user 
sudo: has no permission so it should ask the root to access 
sudo  apt  Firefox.sh
pacman(advanced package manager)
apt for kali depending on the distribution of Linux
pacman -s 
script( written commands)
bash
shell what it translates the commands
to use two commands at once ls (||) filename
ping google.com ( to check if the server working or not
recap
 Linux Recap
 1. User Management in Linux
Linux has two main types of users:
Normal User → limited access

Root User → full control of the system

To perform admin tasks, we use sudo (SuperUser Do).

 Example:
sudo apt update 
 This runs the command with root privileges.
 
 3. Package Installation (Package Managers)

Package managers are used to install and manage software.

APT → used in Kali Linux / Ubuntu

sudo apt install firefox 

PACMAN → used in Arch Linux

sudo pacman -S firefox 

PKG → used in Termux (Android)

pkg install python 

 All do the same job, but used in different systems.
 
 5. Software & Script Installation
script is a file that contains a list of commands that are executed automatically

instead of typing commands one by one,you put them in a file and run it once.

Software can be installed using package managers or scripts.
 Example (script execution):

chmod +x script.sh ./script.sh 

 chmod +x makes the script executable.
 
 8. Linux Shell

The shell is where we type commands to interact with the system.

 Example commands:
 
ls cd Documents pwd 

 These help navigate files and directories.
 
 10. Processes & Management
 11. 
A process is a running program.

 Examples:
 
ps aux top htop 

 To kill a process:
kill PID 
 13. Redirection & Piping
 
Redirection ( > ) → send output to a file

ls > files.txt 

Piping ( | ) → send output to another command

ps aux | grep firefox 

14. Useful Commands 

mkdir folder touch file.txt cp file.txt copy.txt mv file.txt newname.txt rm file.txt
week4/day4

Networking
a collection two or more  connected device

# 🌐 Networking – Cybersecurity Notes

---

## ### 1️⃣ Networking
- Networking: Connecting devices to share data  
- Internet: Global network of networks  

### Used For:
- Communication  
- Data transfer  
- Security monitoring  

---

## ### 2️⃣ IP Address (Internet Protocol)
- IP Address: Unique identifier for a device on a network  
- Used for: Sending and receiving data  

### Example:
- 192.168.1.1  

---

## ### 3️⃣ IPv4
- Definition: 32-bit address  
- Format: 4 numbers separated by dots  

### Example:
- 192.168.0.1  

### Range:
- 0.0.0.0 to 255.255.255.255  

### Problem:
- Limited number of addresses  

---

## ### 4️⃣ IPv6
- Definition: 128-bit address  
- Format: Hexadecimal  

### Example:
- 2001:0db8:85a3::8a2e:0370:7334  

### Advantages:
- Huge number of addresses  
- Better security  

### Usage:
- Future internet  

---

## ### 5️⃣ Difference (IPv4 vs IPv6)
- IPv4: Short, limited  
- IPv6: Long, almost unlimited  
- IPv4: Common today  
- IPv6: Growing usage  

---

## ### 6️⃣ Network Classification (By Geographic Coverage)

### 📍 PAN (Personal Area Network)
- Small range (few meters)  
- Example: Bluetooth, phone hotspot  

### 🏠 LAN (Local Area Network)
- Small area (home, school)  
- Example: WiFi network  

### 🏙️ MAN (Metropolitan Area Network)
- City-level network  
- Example: City internet system  

### 🌍 WAN (Wide Area Network)
- Very large (country/continent)  
- Example: Internet  

---

## ### 7️⃣ IP Classes (Very Important)

### 🅰️ Class A
- Range: 1.0.0.0 – 126.0.0.0  
- Default Subnet: 255.0.0.0  
- Hosts: Very large networks  
- Usage: Big organizations  

### 🅱️ Class B
- Range: 128.0.0.0 – 191.255.0.0  
- Default Subnet: 255.255.0.0  
- Hosts: Medium networks  
- Usage: Universities, companies  

### 🅲 Class C
- Range: 192.0.0.0 – 223.255.255.0  
- Default Subnet: 255.255.255.0  
- Hosts: Small networks  
- Usage: Homes, small businesses  

### 🅳 Class D
- Range: 224.0.0.0 – 239.255.255.255  
- Usage: Multicast (group communication)  

### 🅴 Class E
- Range: 240.0.0.0 – 255.255.255.255  
- Usage: Experimental  

---

## ### 8️⃣ Ports (Cybersecurity)
- Port: Communication endpoint  
- Used for: Connecting services on a system  

### Common Ports:
- HTTP: Port 80 → Web traffic → Not secure  
- HTTPS: Port 443 → Secure web  
- FTP: Port 21 → File transfer → Weak security  
- SSH: Port 22 → Remote access  
- DNS: Port 53 → Domain resolution  

---

## ### 9️⃣ Common Vulnerabilities
- Open ports → Attackers can access services  
- Weak services → Example: FTP (no encryption)  
- Misconfigured ports → Easy entry point  

---

## ### 🔴 Red Team (Attackers)
- Scan network → Find open ports  
- Identify vulnerabilities  
- Exploit weak services  

---

## ### 🔵 Blue Team (Defenders)
- Monitor network traffic  
- Close unused ports  
- Detect suspicious activity  

## ### 🧪 Basic Networking Commands (Kali Linux)

### ping
- Check connectivity  
- Example: ping google.com  

### ifconfig
- Show IP address  

### netstat
- Show active connections


