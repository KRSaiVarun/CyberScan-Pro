Shebang: #!/bin/bash indicates that the script should be run in the Bash shell.

Input Check:

bash
Run
if [ -z "$1" ]; then
    echo "usage: $0 <target_url>"
fi
This checks if a target URL is provided as an argument. If not, it prints usage instructions.

Target Assignment:

bash
Run
Target=$1
This assigns the first argument passed to the script to the variable Target.

Scan Start Message:

bash
Run
echo "starting web vulnerability scan on $Target..."
This prints a message indicating the start of the scan.

Nmap Scan:

bash
Run
echo "Running nmap for vulnerability discovery"
nmap -A --script=vuln $Target -oN nmap_scan.txt
This runs nmap with options to enable OS detection, version detection, script scanning for vulnerabilities, and outputs the results to nmap_scan.txt.

Nikto Scan:

bash
Run
echo "Running nikto"
nikto -h $Target -o nikto_scan.txt
This runs nikto, a web server scanner, and saves the results to nikto_scan.txt.

Completion Message:

bash
Run
Copy code
echo "Scan completed. Results are saved in:"
echo " - nmap_scan.txt"
echo " - nikto_scan.txt"
This prints a message indicating that the scans are complete and lists the output files.
