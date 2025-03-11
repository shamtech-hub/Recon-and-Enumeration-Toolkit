# 🛡️ Recon and Enumeration Toolkit

A comprehensive collection of reconnaissance and enumeration tools designed for ethical hacking, penetration testing, and attack surface mapping. This toolkit leverages powerful open-source OSINT utilities to discover subdomains, directories, files, and potential vulnerabilities in web applications and networks.

## 🚀 Features

- **Subdomain Enumeration**
  - [Amass](https://github.com/owasp-amass/amass)
  - [Assetfinder](https://github.com/tomnomnom/assetfinder)
  - [Findomain](https://github.com/findomain/findomain)
  - [Sublist3r](https://github.com/aboul3la/Sublist3r)
  - [SecurityTrails](https://securitytrails.com/)
  
- **Directory and File Bruteforcing**
  - [Dirsearch](https://github.com/maurosoria/dirsearch)
  - [FFUF](https://github.com/ffuf/ffuf)
  
- **Vulnerability Scanning and Exploitation**
  - [SSRFmap](https://github.com/swisskyrepo/SSRFmap)
  - [Sqlmap](https://github.com/sqlmapproject/sqlmap)

- **Parameter Discovery**
  - [ParamSpider](https://github.com/devanshbatham/paramspider)
  
- **Historical Data Gathering**
  - [Waybackurls](https://github.com/tomnomnom/waybackurls)

## 🛠️ How to Use

### Prerequisites
- Python 3.x
- Go (for tools like FFUF, Assetfinder, etc.)
- Git
- Basic Linux/Unix terminal knowledge

### Installation
```bash
git clone https://github.com/<your-username>/Recon-and-Enumeration-Toolkit.git
cd Recon-and-Enumeration-Toolkit
```

You can then navigate to each tool's folder and follow the respective installation instructions. Most tools can be installed by:
```bash
pip install -r requirements.txt
```
or
```bash
go install <tool>
```

## 📝 Usage

Each tool serves a specific purpose in reconnaissance or enumeration. Here's an example workflow:

1. **Subdomain Enumeration**
   ```bash
   amass enum -d target.com
   assetfinder --subs-only target.com
   findomain -t target.com
   sublist3r -d target.com
   ```

2. **Directory Bruteforcing**
   ```bash
   dirsearch -u https://target.com -e php,html
   ffuf -u https://target.com/FUZZ -w wordlist.txt
   ```

3. **Vulnerability Discovery**
   ```bash
   sqlmap -u "https://target.com/page.php?id=1" --dbs
   ssrfmap -l urls.txt -p '/endpoint?url='
   ```

4. **Parameter Discovery and Historical Data**
   ```bash
   paramspider --domain target.com
   waybackurls target.com
   ```

## ⚠️ Disclaimer
This toolkit is for **educational purposes** and authorized **penetration testing** only. Do **not** use it for unauthorized activities. The developer is not responsible for any misuse.

## 👨‍💻 Author
**Sham Prakash R**  
[LinkedIn](https://www.linkedin.com/in/sham-prakash-337b23250) | [GitHub](https://github.com/shamtech-hub)
