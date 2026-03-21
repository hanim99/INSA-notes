# INSA-notes
week1
Downloading Vbox and Kali Linux

Linux
VirtualBox is a virtualization software developed by  that allows users to run multiple operating systems on a single computer. It creates virtual machines where different systems can be installed and tested safely without affecting the main system.
Kali Linux is a Debian-based Linux distribution developed by . It is widely used for cybersecurity, penetration testing, and ethical hacking. Kali Linux comes pre-installed with many security tools used for network analysis, vulnerability testing, and digital forensics.
VirtualBox is commonly used to run Kali Linux on a PC, making it easy for learners and professionals to practice cybersecurity in a safe and controlled environment.


Week 3
Linux Commands
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
