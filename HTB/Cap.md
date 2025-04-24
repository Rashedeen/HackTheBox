### CAP Machine
A simulated penetration test on the "Cap" machine from Hack The Box, focusing on common vulnerabilities in web applications, network traffic, and Linux capabilities.

### 1. Reconnaissance

![VirusTotal Analysis](images/virustotal-results.png)
> **Figure 5:** Threat intelligence report of malicious files via VirusTotal.

- Performed an Nmap scan.
- Identified open ports:
  - `Port 80`: HTTP (Web Application)
  - `Port 21`: FTP
  - `Port 22`: SSH (requires credentials)

---

### 2. Enumeration

![VirusTotal Analysis](images/virustotal-results.png)
> **Figure 5:** Threat intelligence report of malicious files via VirusTotal.

- Accessed the web app at `http://10.10.10.245`.
- Downloaded and analyzed `.pcap` file.
- Discovered credentials transmitted over unencrypted HTTP.

---

### 3. Exploitation
- SSH access granted using credentials:
  ```bash
  ssh nathan@10.10.10.245
