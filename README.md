# aaayafuj_osint_scanner.sh
🖥️ How to Use
1️⃣ Save the script as aaayafuj_osint_scanner.sh.
2️⃣ Make it executable:

    ```bash
      chmod +x aaayafuj_osint_scanner.sh
3️⃣ Run it with an IP or domain:

    ```bash
    ./aaayafuj_osint_scanner.sh 8.8.8.8
    or
    ./aaayafuj_osint_scanner.sh example.com
🔧 Requirements

* Ensure you have the following installed:

    ```bash
       sudo apt install nmap curl jq whois dnsutils traceroute -y  # Debian/Ubuntu
       sudo yum install nmap curl jq whois bind-utils traceroute -y  # RHEL/CentOS
       brew install nmap curl jq whois bind traceroute  # macOS

# 📌 Important Notes
* Do not scan targets without permission—unauthorized scanning is illegal in many regions.
* Uses real security APIs for threat intelligence and passive OSINT.
* Provides accurate information for security research & penetration testing.
 
💻 Now you have a real OSINT & reconnaissance tool!

🛠️ What aaayafuj_osint_scanner.sh Can Do & How It Works
🔍 What Can This Tool Do?
This tool is an OSINT (Open Source Intelligence) and Reconnaissance scanner that helps gather information about IP addresses and domains. It automates multiple security checks and network scans, making it useful for ethical hacking, penetration testing, and security research.

⚙️ How Does It Work?
The tool takes an IP address or domain as input and performs various OSINT operations, including:

1️⃣ Basic Information Gathering
* ✔ Whois Lookup – Finds owner, ISP, and registration details of a domain or IP.
* ✔ DNS Lookup – Retrieves all DNS records (A, MX, TXT, etc.).
* ✔ Reverse DNS Lookup – Checks if the IP is linked to any domain.

How?

Uses whois, dig, and host commands to extract domain/IP details.

2️⃣ Geolocation & ISP Information
* ✔ Finds the physical location of an IP (Country, City, Latitude/Longitude).
* ✔ Identifies the ISP (Internet Service Provider).

How?

Uses curl to query ip-api.com, which provides geolocation data.

3️⃣ Nmap Scans (Network Security Analysis)
* ✔ Basic Port Scan – Scans open ports to detect running services.
* ✔ Aggressive Scan – Performs detailed OS detection, script scanning, and traceroute.
* ✔ Specific Port Scan – Checks common web & database ports (21, 22, 80, 443, 3306).
* ✔ Vulnerability Scan – Uses Nmap scripts to find security vulnerabilities.

How?

Uses nmap with different options:

* -sV for service detection.
* -A for aggressive mode.
* -p for port-specific scans.

--script vuln to check for vulnerabilities.

4️⃣ Threat Intelligence Lookups
* ✔ Checks if the IP is blacklisted for hacking, malware, or spamming.
* ✔ Looks up security reports related to the IP from threat databases.

How?

Uses curl to query AbuseIPDB and AlienVault OTX APIs.

5️⃣ Traceroute (Network Path Tracking)
* ✔ Shows the path data takes from your device to the target.
* ✔ Identifies network hops, delays, and possible firewalls.

How?

Uses traceroute to trace the path between you and the target.

🚀 How to Use It?
1️⃣ Run the script with an IP or domain:

    ```bash
    chmod +x aaayafuj_osint_scanner.sh
    ./aaayafuj_osint_scanner.sh 8.8.8.8
    ./aaayafuj_osint_scanner.sh example.com

* 2️⃣ The script automatically performs all OSINT and network analysis steps.
* 3️⃣ Results are displayed in real-time, categorized for easy reading.

📌 Why Is This Tool Useful?
✅ Saves time by automating multiple security checks.
✅ Gathers deep intelligence on IP addresses, domains, networks, and threats.
✅ Helps cybersecurity professionals in penetration testing and ethical hacking.
✅ Detects potential vulnerabilities before attackers do.
