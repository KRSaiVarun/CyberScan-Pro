# Web Vulnerability Scanner - `vuln_scan.sh`

A simple yet powerful Bash script for scanning web servers for common vulnerabilities using **Nmap** and **Nikto**. Ideal for quick assessments, automation, and penetration testing practice.

## 📌 Features

- 🔍 Vulnerability scanning using Nmap scripts
- 🛡️ Web server analysis using Nikto
- 🎯 Target URL input
- 🚀 Quick and Full scan modes
- 📁 Organized output directory with timestamped reports
- 🧪 Verbose mode for debugging
- 📜 Help and usage documentation
- ✅ Tool availability and input validation

---

## ⚙️ Requirements

- `bash`
- [`nmap`](https://nmap.org/) (with `--script=vuln` support)
- [`nikto`](https://cirt.net/Nikto2)

Install on Debian-based systems:

```bash
sudo apt update
sudo apt install nmap nikto -y


## 📥 Installation

Clone this repository:

```bash
git clone https://github.com/<your-username>/<repo-name>.git
cd <repo-name>
chmod +x vuln_scan.sh
```

---

## 🛠️ Usage

### Basic Scan

```bash
./vuln_scan.sh example.com
```

### Quick Scan (Common Ports)

```bash
./vuln_scan.sh example.com --quick
```

### Full Scan with Verbose Output

```bash
./vuln_scan.sh https://example.com --full --verbose
```

### Custom Output Directory

```bash
./vuln_scan.sh example.com --output /tmp/scan_results
```

### Help

```bash
./vuln_scan.sh --help
```

---

## 📂 Output

* `nmap_scan.txt`: Nmap scan result
* `nikto_scan.txt`: Nikto web server report
* `scan_summary.txt`: Optional consolidated summary
* All reports stored in the specified or default output directory with timestamps

---

## 🚨 Disclaimer

This script is intended for **educational** and **authorized penetration testing** only. Do **NOT** scan websites or systems you don't own or have permission to test.

---

## 🧑‍💻 Author

**KR Sai Varun**
[GitHub](https://github.com/KRSaiVarun)
Email: `krsaivarun@gmail.com`

---

## 📃 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

````

---

### ✅ Next Steps

1. Replace `<KR Sai Varun>` and `<CyberScan-Pro>` with your actual GitHub username and repository name.
2. Save the above content as `README.md` in your project root directory.
3. Commit and push to GitHub:

```bash
git add README.md
git commit -m "Add README with usage and documentation"
git push origin main
````

