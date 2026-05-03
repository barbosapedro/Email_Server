# Email\_Server

Self-hosted email server lab — Postfix, Dovecot, DKIM/SPF/DMARC, Fail2Ban, ClamAV. Ubuntu Server 24.04



Designed to simulate a production environment for 50–200 users.







Goals:



\- Build a fully functional corporate email server using open-source tools

\- Implement modern email authentication (SPF, DKIM, DMARC)

\- Harden the server against real-world threats (brute force, spam, phishing, malware)



Stack:



| OS | Ubuntu Server 22.04 LTS VM | Host system Windows 11|

| Client | Thunderbird |

| MTA | Postfix | Send/receive email (SMTP) |

| MDA | Dovecot | Deliver \& store email (IMAP) |

| DNS | BIND9 | Local domain resolution |

| Auth | SPF + DKIM + DMARC | Anti-spoofing |

| IDS | Fail2Ban | Brute-force protection |

| Antivirus | ClamAV |

| Anti-spam | SpamAssassin | Spam filtering |











Implementation Phases:



\- \[x] Phase 0 — Environment Setup

\- \[ ] Phase 1 — DNS with BIND9

\- \[ ] Phase 2 — Postfix + Dovecot + Thunderbird

\- \[ ] Phase 3 — TLS Encryption

\- \[ ] Phase 4 — SPF / DKIM / DMARC

\- \[ ] Phase 5 — Fail2Ban, ClamAV, SpamAssassin

\- \[ ] Phase 6 — Mailcow Integration















Security Principles Applied (CIA):



\*\*Confidentiality\*\* — TLS on all connections, authenticated SMTP only  

\*\*Integrity\*\* — DKIM cryptographic signing, DMARC policy enforcement  

\*\*Availability\*\* — Fail2Ban, firewall rules, queue management









