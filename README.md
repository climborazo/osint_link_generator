# 🔍 Osint Link Generator

<div align="center">

![License](https://img.shields.io/badge/license-MIT-blue.svg)
![Version](https://img.shields.io/badge/version-1.0.0-green.svg)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?logo=html5&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?logo=javascript&logoColor=black)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?logo=css3&logoColor=white)

**A powerful, privacy focused Osint enumeration toolkit for rApid intelligence gathering and threat analysis**

[Features](#-features) • [Getting Started](#-getting-started) • [Documentation](#-documentation) • [Contributing](#-contributing)

</div>

---

## 📋 Overview

**Osint Link Generator** is a sophisticated, client side intelligence aggregation tool designed for security researchers, threat analysts, and Osint practitioners. Built with zero backend dependencies, it generates targeted query Urls across 40+ intelligence platforms, enabling seamless pivoting during investigations.

### 🎯 Key Characteristics

- **🔒 Privacy First Architecture**: All processing occurs client side—no data transmission, no telemetry, no logs
- **⚡ Zero Latency**: Instant link generation without Api rate limits or authentication requirements
- **🎨 Optimized UX**: Dark-themed interface with intuitive tab-based navigation
- **📦 Portable**: Single HTML file—works offline, requires no installation or dependencies
- **🔧 Extensible**: Modular design allows easy addition of new intelligence sources

---

## ✨ Features

### 🗂️ Intelligence Categories

<table>
<tr>
<td width="50%">

**Network Intelligence**
- IP reputation & geolocation
- ASN/BGP path analysis
- CIDR block enumeration
- SSL/TLS certificate transparency
- Exposure surface mapping

</td>
<td width="50%">

**Domain Intelligence**
- WHOIS & DNS enumeration
- Subdomain discovery
- Mail security (SPF/DMARC/DKIM)
- Malicious Url detection
- Historical DNS records

</td>
</tr>
<tr>
<td width="50%">

**Threat Intelligence**
- Vulnerability databases (CVE/NVD)
- Malware hash analysis
- Exploit research platforms
- IoC reputation scoring
- Blacklist verification

</td>
<td width="50%">

**Entity Intelligence**
- Corporate entity lookup
- Breach/leak databases
- Social media Osint
- Personnel enumeration
- Geographic reconnaissance

</td>
</tr>
</table>

### 🛠️ Supported Intelligence Platforms

<details>
<summary><b>Search Engines & Aggregators</b> (9 platforms)</summary>

- Shodan
- Censys
- FOFA
- ZoomEye
- LeakIX
- Netlas
- Onyphe
- GreyNoise
- BinaryEdge

</details>

<details>
<summary><b>Threat Intelligence</b> (12 platforms)</summary>

- VirusTotal
- IBM X-Force Exchange
- AlienVault OTX
- AbuseIPDB
- Talos Intelligence
- Hybrid Analysis
- MalwareBazaar
- Urlhaus
- PhishTank
- IPVoid
- UrlVoid
- Spamhaus

</details>

<details>
<summary><b>Vulnerability Research</b> (5 platforms)</summary>

- NVD (National Vulnerability Database)
- MITRE CVE
- Vulners
- Exploit-DB
- CVE Details

</details>

<details>
<summary><b>Infrastructure Analysis</b> (8 platforms)</summary>

- BGP.HE.net
- RIPE Stat
- BGP Tools
- SecurityTrails
- DomainTools
- MXToolbox
- ViewDNS
- DNSViz

</details>

<details>
<summary><b>Breach Intelligence</b> (3 platforms)</summary>

- Have I Been Pwned
- Dehashed
- LeakIX

</details>

<details>
<summary><b>Business & Corporate</b> (4 platforms)</summary>

- OpenCorporates
- Crunchbase
- LinkedIn
- Italian Business Register

</details>

---

## 🚀 Getting Started

### Prerequisites

- Modern web browser (Chrome 90+, Firefox 88+, Safari 14+, Edge 90+)
- JavaScript enabled
- Internet connection (for accessing external platforms)

### Installation

#### Method 1: Direct Download

```bash
# Clone the repository
git clone https://github.com/climborazo/Osint_link_generator.git
cd Osint_link_generator

# Open in browser
open index.html  # macOS
xdg-open index.html  # Linux
start index.html  # Windows
```

#### Method 2: Web Server

```bash
# Python 3
python -m http.server 8000

# Navigate to http://localhost:8000
```

#### Method 3: GitHub Pages

Access directly via: `https://climborazo.github.io/Osint_link_generator`

---

## 📖 Documentation

### Tab Reference

#### 1️⃣ **IP Intelligence**

**Input Format**: IPv4 address (e.g., `8.8.8.8`)

**Generated Intelligence**:
- Reputation scoring (AbuseIPDB, Talos, GreyNoise)
- Geolocation mapping
- Open port enumeration (Shodan, Censys)
- Blacklist verification (Spamhaus, SORBS)
- Attack surface analysis (LeakIX, Netlas)
- BGP routing information

**Use Cases**: Malicious IP investigation, infrastructure attribution, hosting provider identification

---

#### 2️⃣ **Domain Intelligence**

**Input Types**:
- **Domain**: `example.com`
- **Subdomain**: `mail.example.com`
- **Url**: `https://example.com/path`

**Domain Analysis**:
- WHOIS registration data
- DNS record enumeration (A, AAAA, MX, TXT)
- Mail security posture (SPF, DMARC, DKIM)
- Historical DNS records
- Certificate transparency logs
- Subdomain discovery

**Subdomain Enumeration**:
- Search engine discovery
- Certificate transparency
- Passive DNS databases

**Url Analysis**:
- Malicious Url detection
- Dynamic analysis sandboxing
- Screenshot capture
- Redirect chain analysis

**Use Cases**: Phishing investigation, domain reputation checks, infrastructure mapping

---

#### 3️⃣ **Company Intelligence**

**Input Types**:
- **Company Name**: `Acme Corporation`
- **VAT Number**: `IT12345678901`
- **Business ID**: Jurisdiction-specific identifiers

**Generated Intelligence**:
- Corporate registration records
- Organizational structure
- Data breach exposure
- Social media presence
- Executive identification

**Use Cases**: Corporate due diligence, supply chain risk assessment, executive profiling

---

#### 4️⃣ **People Intelligence**

**Input Types**:
- **Full Name**: `John Smith`
- **Email**: `john.smith@example.com`
- **Username**: `jsmith123`
- **Phone**: `+1-555-0123`

**Generated Intelligence**:
- Social media enumeration
- Breach database queries
- Professional network analysis
- GitHub/code repository search
- Phone number validation

**Use Cases**: Personnel investigation, social engineering assessment, breach notification

---

#### 5️⃣ **Geolocation Intelligence**

**Input Types**:
- **Address**: `1600 Amphitheatre Parkway, Mountain View, CA`
- **Coordinates**: `37.4224764,-122.0842499`

**Generated Intelligence**:
- Map visualization (Google Maps, OpenStreetMap)
- Reverse geocoding
- Proximity searches
- Street-level imagery

**Use Cases**: Physical security assessment, incident geolocation, facility identification

---

#### 6️⃣ **Osint Advanced**

##### **ASN Analysis**
**Input**: `AS15169` or `15169`

**Intelligence**:
- BGP routing tables
- IP block allocation
- Peering relationships
- Network topology

##### **CIDR Enumeration**
**Input**: `192.168.0.0/24`

**Intelligence**:
- Network-wide scanning
- Asset discovery
- Service enumeration

##### **Hash Analysis**
**Input**: MD5/SHA1/SHA256/SHA512 hash

**Intelligence**:
- Malware identification
- File reputation scoring
- Sandbox analysis reports
- YARA rule matching

##### **Product Vulnerability**
**Input**: `Apache HTTP Server 2.4.49`

**Intelligence**:
- CVE enumeration
- Exploit availability
- Patch recommendations

##### **CVE Research**
**Input**: `CVE-2021-44228`

**Intelligence**:
- Vulnerability details
- CVSS scoring
- Exploit code availability
- Affected versions

**Use Cases**: Threat hunting, vulnerability management, malware analysis, asset inventory

---

## 🔐 Security & Privacy

### Privacy Guarantees

- ✅ **No Server-Side Processing**: All operations occur in your browser
- ✅ **No Data Transmission**: Inputs never leave your machine until you click a generated link
- ✅ **No Tracking**: Zero analytics, cookies, or fingerprinting
- ✅ **No Storage**: No localStorage, sessionStorage, or IndexedDB usage
- ✅ **Open Source**: Fully auditable codebase

### Security Considerations

⚠️ **Important Notes**:
- Generated links direct to third-party platforms with their own privacy policies
- Some platforms may require authentication or Api keys
- Rate limiting may apply on external services
- Always verify sensitive intelligence through multiple sources

---

## 🎨 Technical Architecture

### Technology Stack

```
┌─────────────────────────────────────┐
│         User Interface Layer        │
│    (Html 5 + Css 3 + Vanilla Js)      │
├─────────────────────────────────────┤
│      Input Processing Layer         │
│  (Validation + Sanitization +       │
│   Encoding + Url Construction)      │
├─────────────────────────────────────┤
│      Link Generation Engine         │
│   (Template based Url builder)      │
└─────────────────────────────────────┘
```

### Key Features

- **Modular Design**: Each intelligence category isolated in separate modules
- **Input Sanitization**: Automatic encoding for special characters and Base64 requirements
- **Responsive Layout**: Optimized for 1920×1080 displays
- **Dark Theme**: Reduced eye strain for extended investigations

### Browser Compatibility

| Browser | Minimum Version | Status |
|---------|----------------|--------|
| Chrome  | 90+ | ✅ Fully Supported |
| Firefox | 88+ | ✅ Fully Supported |
| Safari  | 14+ | ✅ Fully Supported |
| Edge    | 90+ | ✅ Fully Supported |
| Opera   | 76+ | ✅ Fully Supported |

---

## 🤝 Contributing

Contributions are welcome! Please follow these guidelines:

### Adding New Intelligence Sources

1. Fork the repository
2. Add platform Url template to appropriate section
3. Update Readme documentation
4. Submit pull request with description

### Reporting Issues

- Use GitHub Issues for bug reports
- Include browser version and reproduction steps
- Provide sample inputs (sanitized if sensitive)

### Feature Requests

- Check existing issues to avoid duplicates
- Describe use case and expected behavior
- Suggest implementation if applicable

---

## 📄 License

This project is licensed under the Gnu Gpl Version 3 License - See the [LICENSE](LICENSE) file for details.

---

## 🙏 Acknowledgments

- Intelligence platform operators for providing public query interfaces
- Osint community for methodology development
- Security researchers for continuous feedback

---

## ⚠️ Disclaimer

This tool is intended for legitimate security research, threat intelligence, and Osint investigations. Users are responsible for compliance with applicable laws and platform terms of service. The authors assume no liability for misuse.

---

<div align="center">

**climborazo**

- GitHub: [@climborazo](https://github.com/climborazo)

</div>
