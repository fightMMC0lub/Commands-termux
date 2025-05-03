# 📱 Termux Commands 

Welcome to the **Termux Commands Repository** — a curated collection of useful commands for beginners and advanced users alike. Whether you're just starting with Termux or diving into deeper system and network-level tasks, this guide has you covered.

---

## 📌 Table of Contents

1. [Introduction](#introduction)  
2. [Installation & Setup](#installation--setup)  
3. [Basic Commands](#commands/basic.md)  
4. [Package Management](#commands/packages.md)  
5. [File Management](#file-management)  
6. [System Information](#system-information)  
7. [Networking Tools](#networking-tools)  
8. [Development Tools](#development-tools)  
9. [Hacking & Pentesting Tools](#hacking--pentesting-tools)  
10. [Useful Scripts & Tips](#useful-scripts--tips)  


---

## 📖 Introduction

**Termux** is a powerful terminal emulator for Android that gives you access to a Linux environment on your phone. This repository serves as a reference guide with categorized command examples to help you unlock Termux’s full potential.

---

## 🔧 Installation & Setup

Install Termux from [F-Droid](https://f-droid.org/en/packages/com.termux/) (recommended for latest updates):

pkg update && pkg upgrade
pkg install git curl wget
termux-setup-storage


# Termux Commands Reference Guide

A comprehensive list of Termux commands for beginners and advanced users.

---

## Termux Basic Commands

- `cat <file>`: Display the contents of a file.  
- `termux-setup-storage`: Grant Termux access to the Android file system.  
- `clear`: Clear the terminal screen.  
- `pwd`: Print the current working directory.  
- `ls`: List files and directories.  
- `cd <directory>`: Change to a specified directory.  
- `mkdir <directory_name>`: Create a new directory.  
- `touch <file>`: Create a new empty file.  
- `rm <file>`: Delete a file.  
- `mv <source> <destination>`: Move or rename files.  
- `cp <source> <destination>`: Copy files or directories.  

---

## Basic Package Management Commands

- `pkg update`: Update package lists from repositories.  
- `pkg upgrade`: Upgrade all installed packages.  
- `pkg install <package_name>`: Install a specific package.  
- `pkg uninstall <package_name>`: Uninstall a specific package.  
- `pkg search <query>`: Search for a package by name or keyword.  
- `pkg show <package_name>`: Show detailed information about a specific package.  
- `apt list --installed`: List all installed packages.  
- `pkg list-all`: List all available packages.  
- `pkg autoclean`: Remove unnecessary packages.  

---

## Termux Storage Commands

- `ls /sdcard`: List files in the shared storage.  
- `find <directory> -name <file>`: Find files in a directory by name.  
- `tar -cvf <archive_name>.tar <directory>`: Create a tarball from a directory.  
- `tar -xvf <archive_name>.tar`: Extract files from a tarball.  

---

## File and Directory Commands

- `stat <file>`: Show file or directory status.  
- `ls`: List files and directories.  
- `pwd`: Print the current working directory.  
- `cd <directory>`: Change to a specified directory.  
- `cp <source> <destination>`: Copy files or directories.  
- `mv <source> <destination>`: Move or rename files or directories.  
- `rm <file>`: Remove a specified file.  
- `rmdir <directory>`: Remove an empty directory.  
- `touch <file>`: Create a new empty file.  
- `cat <file>`: Display the contents of a file.  
- `head <file>`: Show the first 10 lines of a file.  
- `tail <file>`: Show the last 10 lines of a file.  

---

## Text Editing Commands

- `nano <file>`: Edit files with the Nano editor.  
- `vim <file>`: Edit files with the Vim editor.  
- `cat <file>`: Display the contents of a file.  
- `sed 's/old/new/g' <file>`: Replace ‘old’ with ‘new’ in a file.  
- `grep <pattern> <file>`: Search for a specific pattern in a file.  

---

## System Information and Monitoring

- `uname -a`: Display system information.  
- `top`: Show running processes and resource usage.  
- `htop`: An improved version of top (requires installation).  
- `df -h`: Display disk usage in human-readable format.  
- `du -sh <directory>`: Show the size of a specified directory.  
- `free`: Show memory usage.  
- `termux-info`: Display information about the Termux environment.  
- `lscpu`: Display CPU architecture information.  
- `lsusb`: List USB devices connected to your system.  
- `lspci`: List PCI devices (may not work on all devices).  

---

## Network Commands

- `ping <host>`: Test connectivity to a specified host.  
- `ifconfig`: Show network interfaces and configurations.  
- `curl <URL>`: Download a file from a specified URL.  
- `wget <URL>`: Fetch files from the web using wget.  
- `ssh user@host`: Connect to a remote system using SSH.  
- `traceroute <host>`: Trace the route to a network host.  
- `netstat`: Display network connections and listening ports.  
- `nslookup <domain>`: Query the DNS for a specific domain.  

---

## Process Management Commands

- `fg <job_id>`: Bring a background job to the foreground.  
- `ps`: List running processes.  
- `top`: Show running processes and resource usage.  
- `htop`: An improved version of top (requires installation).  
- `kill <pid>`: Terminate a process by its PID.  
- `killall <process_name>`: Terminate all processes with the given name.  
- `jobs`: List active jobs.  
- `bg <job_id>`: Resume a job in the background.  

---

## Scripting and Development Commands

- `python <script.py>`: Run a Python script.  
- `bash <script.sh>`: Run a Bash script.  
- `gcc <file.c>`: Compile C code.  
- `g++ <file.cpp>`: Compile C++ code.  
- `node <file.js>`: Run a Node.js script.  
- `chmod +x <script.sh>`: Make a script executable.  
- `./<script.sh>`: Execute a script in the current directory.  

---

## Termux API Commands

- `termux-battery-status`: Get battery status and information.  
- `termux-location`: Get the current device location (GPS).  
- `termux-vibrate`: Make the device vibrate.  
- `termux-wifi-scaninfo`: Get information about Wi-Fi networks.  
- `termux-telephony-call <phone_number>`: Make a phone call from the terminal.  
- `termux-telephony-sms-send <phone_number> "<message>"`: Send an SMS.  
- `termux-camera-photo <file_path>`: Take a photo using the device camera.  

---

## Termux Tools Commands

- **Nmap**: Network exploration and security auditing tool.  
  - `nmap <target>`: Scan a target for open ports and services.  

- **Metasploit**: Penetration testing framework.  
  - `msfconsole`: Start the Metasploit console.  

- **Hydra**: Network login cracker.  
  - `hydra -l <username> -P <password_list> <protocol>://<target>`: Perform a brute force attack.  

- **Nikto**: Web server scanner.  
  - `nikto -h <target>`: Scan a web server for vulnerabilities.  

- **Aircrack-ng**: Wi-Fi network security toolset.  
  - `airmon-ng`: Start monitor mode.  
  - `airodump-ng <interface>`: Capture packets on a specified interface.  

- **sqlmap**: Automatic SQL injection tool.  
  - `sqlmap -u <url> --dbs`: Enumerate databases.  

- **Wget**: File download tool.  
  - `wget <URL>`: Download a file from the web.  

- **Curl**: Data transfer tool.  
  - `curl -O <URL>`: Download a file from the web.  

---

## File Running Commands

- `sh <script.sh>`: Run a shell script.  
- `python <script.py>`: Execute a Python script.  
- `ruby <script.rb>`: Run a Ruby script.  
- `perl <script.pl>`: Execute a Perl script.  
- `node <script.js>`: Run a Node.js script.  
- `java <ClassName>`: Run a compiled Java program.  
- `./<executable>`: Execute a compiled executable in the current directory.  
- `bash <script.sh>`: Execute a Bash script directly.  

---

## Git Commands

- `git clone <repository_url>`: Clone a remote repository.  
- `git init`: Initialize a new Git repository.  
- `git add <file>`: Stage files for commit.  
- `git commit -m "message"`: Commit staged changes.  
- `git push origin <branch>`: Push commits to a remote branch.  
- `git pull`: Fetch and merge changes from remote.  
- `git branch`: List all branches.  
- `git checkout <branch>`: Switch branches.  

---

## Other Useful Commands

- `df -i`: Show inode usage.  
- `clear`: Clear the terminal screen.  
- `history`: Show the command history.  
- `alias <name>=<command>`: Create a shortcut for a command.  
- `exit`: Close the Termux session.  
- `date`: Show the current date and time.  
- `echo "text"`: Print “text” to the terminal.  

---
