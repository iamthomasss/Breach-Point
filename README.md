# Breach-Point


## Objective

The objective of this project is to develop an automated phase of penetration testing which include network reconnaissance, credential brute-forcing, exploit preparation, payload creation and data exfiltration. 


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



## Skills Learned

1. 


## Tools Used

1. Nmap + NSE (default, brute, vuln scripts) & Searchsploit
2. Hydra (SSH, RDP, FTP, SMB modules)
3. Metasploit (msfconsole & msfvenom)


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
