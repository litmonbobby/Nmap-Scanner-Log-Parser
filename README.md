# Nmap Scanner & Log Parser

This Python CLI tool performs a fast TCP SYN scan on a target machine using Nmap, parses the output, and highlights potentially risky ports and services. It's designed to help junior security engineers or students practice basic network scanning and log management.

## Features

- Fast Nmap scan (`-sS -T4 -Pn`) execution
- Parses open ports and detected services from output
- Flags known risky ports like Telnet (23), SMB (445), RDP (3389)
- Color-coded terminal output for easier readability
- Automatically saves results to a timestamped log file

## Skills Demonstrated

- Python scripting
- Subprocess handling
- Regex & output parsing
- Basic network security concepts
- Log creation and file management

## Example Usage

```bash
$ python scanner.py --target 192.168.1.100
Sample Output
text
Copy
Edit
[+] Open Port: 22/tcp (ssh)
[+] Open Port: 80/tcp (http)
[!] Potential risk: Port 23/tcp (telnet)
[+] Log saved to scan_192_168_1_100_20250428_1035.log
Setup
Make sure Nmap is installed and available in your system PATH

Clone this repo and run the script:

bash
Copy
Edit
git clone https://github.com/your-username/nmap-scanner-log-parser.git
cd nmap-scanner-log-parser
python scanner.py --target <IP>
Requirements
Python 3.6+

Nmap installed locally

Author: Bobby Litmon
Contact: litmonbobby@gmail.com
