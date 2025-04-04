# 🧰 OSINT Toolkit 

This repository contains a curated set of tools and automation scripts for public web data collection and analysis using Crawlbase (formerly ProxyCrawl) and other open-source solutions. The toolkit is designed for OSINT, cybersecurity research, social media analysis, and general web scraping.

> ⚠️ Disclaimer: This project is for educational and research purposes only. Always follow local laws and respect target websites' terms of service and robots.txt policies.

---

## 🚀 Scenario

This toolkit is useful for:

- Gathering public data from web sources
- Passive reconnaissance for domains and users
- Metadata and document analysis
- Social media and geo-analysis
- Creating reports and visualizations

All tools are open-source or offer free tiers, and you can combine them in pipelines for automation.

---

## 🔧 Tool List

### 🕷 Crawlbase (formerly ProxyCrawl)
- **Purpose**: Bypass bot detection to safely extract public web data
- **Link**: [https://crawlbase.com](https://crawlbase.com)

### 🌎 theHarvester
- **Purpose**: Email, subdomain, IP, and URL recon
- **Repo**: [https://github.com/laramies/theHarvester](https://github.com/laramies/theHarvester)

### 🌐 Amass
- **Purpose**: In-depth domain enumeration
- **Repo**: [https://github.com/owasp-amass/amass](https://github.com/owasp-amass/amass)

### 🧠 SpiderFoot
- **Purpose**: Fully automated OSINT recon tool
- **Repo**: [https://github.com/smicallef/spiderfoot](https://github.com/smicallef/spiderfoot)

### 🐦 Social Analyzer
- **Purpose**: Social media username checker and analytics tool
- **Repo**: [https://github.com/qeeqbox/social-analyzer](https://github.com/qeeqbox/social-analyzer)

### 🛰 Holehe
- **Purpose**: Check email address usage on 100+ websites/services
- **Repo**: [https://github.com/megadose/holehe](https://github.com/megadose/holehe)

### 🔍 ExifTool
- **Purpose**: Extract metadata (e.g., from images, documents)
- **Site**: [https://exiftool.org](https://exiftool.org)

### 🧭 Metabigor
- **Purpose**: Passive recon using search engines and APIs
- **Repo**: [https://github.com/j3ssie/metabigor](https://github.com/j3ssie/metabigor)

### 🌐 Censys CLI
- **Purpose**: Search internet-wide for devices and domain metadata
- **Repo**: [https://github.com/censys/censys-python](https://github.com/censys/censys-python)

### 💻 Shodan CLI
- **Purpose**: Search connected assets by IP, ports, devices, etc.
- **Site**: [https://cli.shodan.io](https://cli.shodan.io)

### ➕ Bonus Tools
- **Maltego CE** – Link analysis
- **Recon-ng** – Recon automation framework
- **FOCA** – Document metadata analysis

---

## ⚙ Usage Flow Example

```bash
# 1. Enumerate subdomains
amass enum -d target.com -o subdomains.txt

# 2. Get public emails and hosts from target domain
theHarvester -d target.com -b all

# 3. Lookup social media presence
python social-analyzer -u "target_username"

# 4. Extract metadata from a file
exiftool file.jpg

# 5. Crawl a site with Crawlbase
curl "https://api.crawlbase.com/?token=YOUR_API_KEY&url=https://target.com"
