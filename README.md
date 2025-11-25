# Breach-Point


## Objective

The objective of this project is to develop a simple and effective port scanning tool that identify which ports are open on a target system. This tool aims to give us an understanding of network security by utilizing Python’s socket module to probe systems and retrieve service banners, providing insights into potential vulnerabilities.


## Overview

This project involves creating a port scanning tool used to probe a target system or network to identify which ports are open and listening for connections. This project introduces beginners to key cybersecurity concepts like networking, sockets, and TCP/UDP communication while strengthening Python skills.

### Features of the Port Scanner:
1. Accepts a target IP address or hostname.
2. Allows the user to specify a range of ports to scan.
3. Scans for open TCP or UDP ports.
4. Prints the results (open ports) in a user-friendly format.
5. Retrieve and display service banners for open ports.
6. Save scan results to a file for later analysis.
7. Add functionality to ping a range of IPs to discover live hosts.
8. Speed up scanning by checking multiple ports simultaneously (Multi-Threading).


## Skills Learned

1. Implement both TCP and UDP port scanning techniques to identify open services on a target.
2. Mapping port numbers to service names using socket.getservbyport.
3. Learned to use threading module to perform port and ping scanning concurrently, speeding up the scanning process.
4. Learnt to implement thread safety using a 'threading.lock' when updating shared resources.
5. Convert between dotted-decimal IP addresses and their integer representation for easy range iteration.
6. Taking user input for targets, port ranges, and IP ranges.
7. Exporting results to an external file.
8. Using 'try . . . except' blocks to handle potential errors such as network timeouts, unknown services, or failed command execution. 


## Tools Used

1. Socket module
2. Threading module
3. subprocess module
4. input() module
5. open() module


## Screenshots of project

### Using the target IP address to run the port scanner



### Using target Hostname to run the port scanner

