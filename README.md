# FFLANEE: Security Tool for Penetration Testing

FFLANEE is a powerful security tool designed to assist security professionals with various penetration testing tasks. This tool provides functionalities for web pentesting, network pentesting, malware analysis, and more. It is essential to run this tool as root for full access to required features.

### Features
- **Web Pentesting**  
  Perform website vulnerability scans, extract URLs, and more.

- **Network Pentesting**  
  Run network discovery tools such as Ping Sweep, TCP Scan, and Port Scan to map and assess network vulnerabilities.

- **Wireless Pentesting**  
  Tools for testing wireless network security (feature not implemented in this version).

- **Malware Analysis**  
  Analyze malware samples (feature not implemented in this version).

- **DoS & DDoS**  
  Perform Denial of Service (DoS) and Distributed Denial of Service (DDoS) attacks.

- **Security Hardening**  
  Apply security hardening measures to improve system defense.

### Installation
Clone the repository to your local machine:

```bash
git clone https://github.com/SekloSec/FFLANEE.git
cd FFLANEE
```
Ensure you have the necessary dependencies installed:

```bash
pip install -r requirements.txt
```

### Usage

To run FFLANEE, simply execute the Python script:

```bash
sudo python3 fflanee.py
```

### Main Menu

Upon launching, the user will be presented with the following main menu:

```bash
{1}--Web Pentesting
{2}--Network Pentesting
{3}--Wireless Pentesting
{4}--Malware Analysis
{5}--DoS & DDoS
{6}--Security Hardening
{0}--Exit
```

### Web Pentesting Menu

```bash
{1}--Web Crawler
{2}--TCP Scan
{3}--Port Scan
{0}--Back to Main Menu
{99}--Exit
```
**1.** **Web Crawler:** Extract URLs from a given website

**2.** **TCP Scan:** Perform a TCP scan to detect active services on a given IP

**3.** **Port Scan:** Scan specific ports on a target to check for open ports

### Network Pentesting Menu

The Network Pentesting section includes:

```css
{1}--Ping Sweep
{2}--TCP Scan
{3}--Port Scan
{0}--Back to Main Menu
{99}--Exit
```
**1.** **Ping Sweep:** Scan a range of IPs to check which are alive

**2.** **TCP Scan:** Scan specific TCP ports to identify open services

**3.** **Port Scan:** Scan ports for open services on a specific IP

### DoS & DDoS Menu

This section lets you perform DoS or DDoS attacks. (Use responsibly.)

### Security Hardening Menu

This section helps to apply basic security hardening measures to improve system security

### Dependencies

**- requests:** For making HTTP requests to websites

**- beautifulsoup4:** For parsing HTML and extracting data

**- socket:** For networking operations like port scanning and TCP scans

**- threading:** For multi-threading operations like Ping Sweep, TCP Scan, etc

**- collections:** For managing ordered dictionaries during scans

**- time:** For timing operations

### Disclaimer

**FFLANEE** is a penetration testing tool created for educational and ethical hacking purposes only. Always have permission before testing systems that you do not own. Unauthorized access to computer systems is illegal and punishable by law

```rust

This README includes detailed sections for installation, usage, and description of each feature in the tool, making it suitable for GitHub.

```

