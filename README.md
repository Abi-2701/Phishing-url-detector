# Phishing URL Detector

## Overview

Phishing URL Detector is a Python-based cybersecurity tool that analyzes URLs and identifies potential phishing indicators using heuristic-based detection techniques. The tool evaluates multiple risk factors and generates a risk score along with security recommendations.

This project was developed to understand phishing attacks, URL-based threats, and basic threat detection methodologies used in cybersecurity.

---

## Features

### URL Security Analysis

- Detects insecure HTTP connections
- Identifies suspicious keywords commonly used in phishing attacks
- Detects URLs containing IP addresses instead of domain names
- Detects excessive hyphens in URLs
- Identifies URL shortening services
- Detects potential brand impersonation attempts
- Generates a risk score
- Provides security recommendations

---

## Detection Techniques

### Protocol Analysis

Checks whether the URL uses:

- HTTPS (Secure)
- HTTP (Insecure)

### Suspicious Keyword Detection

Detects phishing-related keywords such as:

- login
- verify
- secure
- account
- update
- banking
- password

### IP Address Detection

Example:

http://192.168.1.100/login

Attackers often use IP addresses to hide malicious destinations.

### URL Shortener Detection

Detects:

- bit.ly
- tinyurl.com
- t.co
- goo.gl

### Brand Impersonation Detection

Detects possible impersonation attempts involving brands such as:

- PayPal
- Google
- Facebook
- Amazon
- Microsoft
- Apple

Example:

https://paypa1-login.com

### URL Structure Analysis

Checks:

- URL length
- Excessive hyphens
- Suspicious formatting

---

## Technologies Used

- Python 3
- Regular Expressions (Regex)
- URL Analysis Techniques
- Heuristic-Based Detection

---

## Project Structure

```text
phishing-url-detector/
│
├── phishing_detector.py
├── requirements.txt
├── README.md
│
└── screenshots/
    ├── safe_url.png
    ├── phishing_url.png
    └── ip_based_url.png
```

---

## Installation

Clone the repository:

```bash
git clone https://github.com/Abi-2701/phishing-url-detector.git

cd phishing-url-detector
```

---

## Usage

Run the tool:

```bash
python phishing_detector.py
```

Enter a URL when prompted:

```text
Enter URL: https://github.com
```

---

## Sample Results

### Safe URL

Input:

```text
https://github.com
```

Output:

```text
Risk Score : 0/10
Risk Level : LOW
```

### Suspicious URL

Input:

```text
http://secure-login-update-account.com
```

Output:

```text
Risk Score : 6/10
Risk Level : HIGH
```

### IP-Based URL

Input:

```text
http://192.168.1.100/login
```

Output:

```text
Risk Score : HIGH
Risk Level : HIGH
```

### Medium-Level URL

Input:

```text
http://secure-login-update-account.com
```

Output:

```text
Risk Score : 6/10
Risk Level : HIGH
```
---

## Screenshots

### Safe URL Analysis

![Safe URL](screenshots/safe_url.png)

### Phishing URL Detection

![Phishing URL](screenshots/phishing_url.png)

### IP Address URL Detection

![IP-Based URL](screenshots/ip_based_url.png)

### Medium level URL Detection

![Medium-level URL](screenshots/medium_level_url.png)

---

## Cybersecurity Concepts Demonstrated

- Phishing Detection
- URL Reputation Analysis
- Social Engineering Awareness
- Threat Identification
- Risk Assessment
- Security Scoring
- Reconnaissance Prevention

---

## Learning Outcomes

Through this project, the following cybersecurity concepts were explored:

- Identifying phishing indicators
- Understanding URL-based attacks
- Risk scoring methodologies
- Security-focused Python scripting
- Threat analysis fundamentals

---

## Future Improvements

- Machine Learning-Based Detection
- Domain Reputation Lookup
- WHOIS Integration
- Export Reports (PDF/CSV)
- Real-Time URL Monitoring

---

## Author

**Abishaa**

GitHub: https://github.com/Abi-2701

---

## License

This project is licensed under the MIT License.
