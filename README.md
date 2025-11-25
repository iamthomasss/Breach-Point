# Breach-Point


## Objective

The objective of this project is to develop an automated phase of penetration testing which include network reconnaissance, credential brute-forcing, exploit preparation, payload creation and data exfiltration. 
<br />

## Overview

This project involves a step-by-step process of penetration testing: scan of network, logging each step, and allowing the user to inspect or re-run any phase on demand. It generates a structured output in user-input directory and concludes with a search tool to review the results. 

### Features of the Project:
1. Network Scan: Basic or Full Scan; including service version, weak passwords and vulnerabilities.
2. Attack Paths
   . Weak Credentials: Check for weak passwords in SSH, RDP, FTP and SMB
   . RC File Generation: Allows for user to choose which .rc file to generate
   . Payload Generation: Allows for user to create a payload
   . Data Exfiltration: Allows user to create script for data exfiltration
4. Interactive Search: Allows for user to search through the results/outputs. 
<br />
<br />


## Skills Learned

1. Bash Fundamentals: writing functions, using loops and conditional logic.
2. Input Validation: Using a while loop and a regular expression to validate user input (network format).
3. File and Directory Management: Creating directories, setting default paths, and writing output to files.
4. Command Line Utility Integration: Integrating and controlling multiple command-line tools (Nmap, Hydra, msfconsole, Searchsploit) within a single script.
5. Variable Manipulation: Setting and retriecing environemtn and custom variables.
6. System Information Gathering: Using standard Linux commands like 'ifconfig', 'grep', 'tail', and 'awk' to determine the IP address.
7. Host Discovery: Using '-Pn' (skip host discovery) and scanning a target network range.
8. Port Scanning: Conducting TCP and UDP scans, including comprehensive port scanning (-p- for all ports in full scan).
9. Service Version Detection: Using '-sV' to identify the application running on open ports.
10. OS Detection: Using '-O' to fingerprint the target operating system.
11. Nmap Scripting Engine (NSE): Utilising key NSE script categories:
    . default: Standard scripts for service enumeration
    . brute: check weak/default credentials
    . vuln: detect common vulnerabilities
12. Output Management: Saving Nmap results in multiple formats (-oA) for later analysis.
13. Vulnerability Mapping: Using Searchsploit to cross-reference Nmap XML output against the Exploit-DB database to find known exploits for identified services/versions.
14. Brute-Force Attack: Using Hydra (hydra -L -P) to perform dictionary attacks against common network services using a provided list of usernames and passwords.
15. Resource File Generation: Creating Metasploit Resource Files to automate complex actions such as:
    . Exploiting SSH login
    . Setting up a multi/handler for reverse connections
    . Using the 'local_exploit_suggester' post module.
16. Payload Generation: Using msfvenom to create custom shellcode/executables with specific settings.
17. Data Staging: Generating platform-specific command chains for:
    . Location Sensitive Files: Using 'find' (Linux) or 'dir/findstr' (Windows Powershell) to searh for files containing keywords like "password".
    . Archiving: Compressing files using 'zip' or 'Compress-Archive'.
    . Encoding: In Linux, use 'base64' or in windows using 'certutil -encode'
    . Exfiltration: Generate a command 'scp' to securely copy the encoded datas back to the system. 
<br />
<br />


## Tools Used

1. Nmap + NSE (default, brute, vuln scripts) & Searchsploit
2. Hydra (SSH, RDP, FTP, SMB modules)
3. Metasploit (msfconsole & msfvenom)
<br />
<br />

## Results 

### Network Scan Output
1. Basic and Full scan outputs in gnmap, nmap and xml format
2. Displays of open ports in both TCP/UDP, service versions, weak passwords and vulnerabilities (in both NSE and Searchsploit)

### Weak Credentials Output
1. Hydra brute-force over the services (SSH, RDP, FTP and SMB) against either user lists or default lists; logging each service's results into user's indicated directory

### RC File Generation Output
1. Automates the RC file creation for SSH login scan, handler, or suggester
2. An option to allow the user to choose if they would like to execute the '.rc' file in msfconsole

### Payload Generation
1. Prompts for payload type, LHOST/LPORT, format and filename and saves to chosen directory

### Data Exfiltration
1. Write to a shell script containing OS-specific commands (linux or windows) to look for files containing specific keywords, compress it into a zip file, encode into base64 and ultimately scp to the attacker machine.
<br />
<br />
   
   

## Screenshots of project

### Go to the directory where the script is located in and run the script
<img src="https://i.imgur.com/L595l36.png" height="80%" width="80%" />
<br />
<br />


### Key in the target ip address and output directory name. Next, select whether do you want to do a Basic or Full Scan.
<img src="https://i.imgur.com/35Fnbve.png" height="80%" width="80%" />
<br />
<br />


### Basic Scan in progress
<img src="https://i.imgur.com/6KI43Z3.png" height="80%" width="80%" />
<br />
<br />


### Basic Scan is complete with the information exported to a file. Next, select either attack path to continue or exit. 
<img src="https://i.imgur.com/MVQch2H.png" height="80%" width="80%" />
<br />
<br />


### Weak Credentials Checks Path 
<img src="https://i.imgur.com/nKzHVSS.png" height="80%" width="80%" />
<br />
<br />


### Search through the results/output using keywords/terms
<img src="https://i.imgur.com/AJ7HkSN.png" height="80%" width="80%" />
<br />
<br />


### Automate with Resource File Path
<img src="https://i.imgur.com/C47ZI7A.png" height="80%" width="80%" />
<br />
<br />


### Execute the RC file
<img src="https://i.imgur.com/wiMFb5y.png" height="80%" width="80%" />
<br />
<img src="https://i.imgur.com/XK207LT.png" height="80%" width="80%" />
<br />


### Search through the results/output using '.rc'
<img src="https://i.imgur.com/hfsHqK6.png" height="80%" width="80%" />
<br />
<br />


### Generating a payload
<img src="https://i.imgur.com/akJ1cJs.png" height="80%" width="80%" />
<br />
<br />


### Search through the results/output using 'elf'
<img src="https://i.imgur.com/YPHKSt4.png" height="80%" width="80%" />
<br />
<br />


### Generate Data Exfiltration script containing OS-Specific Commands
<img src="https://i.imgur.com/0Nf5eqx.png" height="80%" width="80%" />
<br />
<br />


### Full Scan in Progress
<img src="https://i.imgur.com/BtnFeOm.png" height="80%" width="80%" />
<br />
<br />


### Full Scan with Searchsploit Analysis is complete with the information exported to a file. Next, select either attack path to continue or exit. 
<img src="https://i.imgur.com/EOB0Iwi.png" height="80%" width="80%" />
<br />
<img src="https://i.imgur.com/maLV81a.png" height=80%" width="80%" />
<br />


### Exiting the script
<img src="https://i.imgur.com/kcuaZSq.png" height="80%" width="80%" />
<br />


### Exported files for analysis 
<img src="https://i.imgur.com/DU1Ad5X.png" height="80%" width="80%" />
<br />
<img src="https://i.imgur.com/2eIt5Mm.png" height="80%" width="80%" />
<br />
<img src="https://i.imgur.com/uTUde6g.png" height="80%" width="80%" />
<br />
