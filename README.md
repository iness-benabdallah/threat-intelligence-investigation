# OSINT & Cyber Threat Intelligence Investigation

### Investigating a suspicious domain linked to macOS malware

This project documents a passive OSINT and Cyber Threat Intelligence investigation into **scope68.com**, a domain reported by URLhaus for distributing malware.

The goal was to understand what was happening behind the domain, examine its infrastructure, identify related indicators of compromise (IoCs), and assess the potential threat.

## What I investigated

- Domain reputation and registration details
- DNS records and associated IP addresses
- Hosting infrastructure and TLS certificate
- Related files and malware indicators
- Hash correlation between URLhaus and VirusTotal
- AMOS (Atomic macOS Stealer) threat intelligence

## Key findings

- The domain was listed on URLhaus as distributing malware.
- VirusTotal reported malicious detections for the domain.
- One URLhaus payload hash matched a VirusTotal report identifying an AMOS-associated macOS executable.
- Additional files were found in VirusTotal's domain relations, but their exact relationship to the identified payload could not be established.

## Methodology & tools

The investigation used publicly available threat intelligence and passive OSINT sources, including:

- **URLhaus** – malicious URL intelligence
- **VirusTotal** – domain, IP and file analysis
- **DNSChecker** – DNS record verification
- **Public threat research** – AMOS malware background

## Repository structure

```text
├── evidence/        # Screenshots supporting the findings
├── indicators/      # Extracted indicators of compromise (IoCs)
├── investigation/   # Final investigation report
└── README.md
```

## Scope & safety

This was a passive investigation using publicly available information. No malware was downloaded or executed, and no unauthorized access was attempted.


