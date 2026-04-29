# Searching Tools

### (1) Shodan
Shodan is often described as a search engine for the Internet of Things (IoT), but that undersells it. Shodan continuously scans the internet, searching for networking equipment, industrial control systems, traffic cameras, and virtually anything else with a public network connection to see what's running and where.
<img src="https://tryhackme-images.s3.amazonaws.com/user-uploads/5f04259cf9bf5b57aed2c476/room-content/5f04259cf9bf5b57aed2c476-1718112514634"/>

### (2) VirusTotal
VirusTotal collates results from over 70 antivirus engines and website scanners into a single interface. Submit a file, a URL, a domain, or a file hash. VirusTotal will tell you whether any of those engines have flagged it as malicious or not.
<img src="https://tryhackme-images.s3.amazonaws.com/user-uploads/5de96d9ca744773ea7ef8c00/room-content/5de96d9ca744773ea7ef8c00-1773875621227.png"/>

### (3) Vulnerability Databases (CVE)
The Common Vulnerabilities and Exposures (CVE) programme is the closest thing the industry has to a universal dictionary of known vulnerabilities.
<img width="726" height="462" alt="image" src="https://github.com/user-attachments/assets/d407cfdc-034c-45e5-a881-03c2cc0eebcf" />

Each confirmed vulnerability is assigned a unique identifier in the format CVE-YEAR-NUMBER, such as **CVE-2025-55182**. If the vulnerability is impactful enough, it may even get a moniker. You may have heard of vulnerabilities such as Heartbleed, React2Shell, and Log4Shell. These vulnerabilities are given a score (CVSS) based on a variety of factors, such as:

   * Impact - What damage can this vulnerability lead to?
   * Complexity - Is the vulnerability easy to exploit or not? 
   * Availability - How likely is it that someone can exploit this?

These identifiers function as a reference point among vendors, researchers, security tools, and documentation, ensuring that everyone discussing a vulnerability refers to the same issue. Websites like ExploitDB compile this information alongside "Proof of Concepts" (PoCs), which are scripts capable of demonstrating the vulnerability.
<img width="873" height="180" alt="image" src="https://github.com/user-attachments/assets/6baecb1d-4e58-4c9b-a046-ec02b5408e22" />

### (4) Technical Documentation (MAN)
#### Product and Tool Documentation
Each major security tool or platform provides its own documentation, which is the most reliable and up-to-date than any third-party tutorials. When you're troubleshooting unexpected behaviour or trying to understand how to use a tool in a certain way, the official documentation should always be your first stop - not your last.

#### Linux Man Pages
Have you ever come across a command-line tool or command that you're not familiar with? Linux MANual pages have got your back. These pages serve as documentation that you can read within your terminal about any command on Linux, and a majority of cybersecurity tooling 

To view the manual page, run **man <command>**. For example:
<img width="614" height="274" alt="image" src="https://github.com/user-attachments/assets/f0b42aa4-e45e-4cf8-a419-6675204b8a3d" />

### (5) GitHub

GitHub can be a great resource for staying updated on the latest threats and vulnerabilities. Researchers often publish proof-of-concept (PoC) code, exploitation tools, and detailed technical reports there, which are usually faster than official channels. 

Searching for a CVE identifier (e.g., CVE-2026-13337) directly on GitHub often reveals repositories containing PoC code, scanner scripts, or detailed analyses of the vulnerability.
