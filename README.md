# 🛡️ Security Testing & Penetration Notes

> A comprehensive community-driven repository of penetration testing techniques, vulnerability assessments, and security research notes.

---

## 📋 Overview

This repository is a curated collection of detailed security testing guides and penetration testing methodologies. It provides hands-on approaches, attack vectors, vulnerability mechanisms, and exploitation techniques for security researchers, bug bounty hunters, and penetration testers.

Whether you're conducting security assessments, preparing for certifications, or expanding your security knowledge, this resource offers structured, practical guidance on identifying and exploiting common web vulnerabilities.

---

## 🚀 Features

- ✅ **Comprehensive Coverage** – Detailed guides for 20+ vulnerability types and attack vectors
- ✅ **Practical Methodology** – Step-by-step exploitation techniques and walkthroughs
- ✅ **Real-World Examples** – Practical payloads, tools, and detection methods
- ✅ **Well-Structured** – Organized with shortcuts, mechanisms, and hunting strategies
- ✅ **Actively Updated** – Community-driven content from security researchers
- ✅ **Tool Integration** – Recommendations for popular penetration testing tools

---

## 📚 Documentation Topics

The repository covers the following security domains:

### Web Application Security

| Vulnerability | File | Description |
|---|---|---|
| **SQL Injection** | [sql-injection.md](sql-injection.md) | SQL injection techniques, exploitation, and bypass methods |
| **Cross-Site Scripting (XSS)** | [xss.md](xss.md) | Stored, reflected, DOM-based, and blind XSS attacks |
| **Cross-Site Request Forgery (CSRF)** | *See respective files* | CSRF attack vectors and defense bypass |
| **Server-Side Template Injection** | [ssti.md](ssti.md) | Template injection vulnerabilities and exploitation |
| **Insecure Deserialization** | [insecure-deserialization.md](insecure-deserialization.md) | Object deserialization exploits and RCE techniques |
| **Open Redirect** | [open-redirect.md](open-redirect.md) | Open redirect vulnerabilities and impact chains |
| **XXE (XML External Entity)** | [xxe.md](xxe.md) | XXE injection, SSRF, and data exfiltration |
| **SSRF (Server-Side Request Forgery)** | [ssrf.md](ssrf.md) | SSRF attacks, cloud metadata exploitation |

### Authentication & Authorization

| Vulnerability | File | Description |
|---|---|---|
| **JWT Vulnerabilities** | [jwt.md](jwt.md) | JWT attack vectors, key recovery, algorithm confusion |
| **OAuth Vulnerabilities** | [oauth.md](oauth.md) | OAuth protocol flaws and implementation bypasses |
| **IDOR (Insecure Direct Object Reference)** | [idor.md](idor.md) | Authorization bypass techniques |

### Advanced Attack Vectors

| Vulnerability | File | Description |
|---|---|---|
| **Remote Code Execution** | [rce.md](rce.md) | RCE techniques across multiple technologies |
| **HTTP Request Smuggling** | [req-smuggle.md](req-smuggle.md) | Request smuggling and desynchronization attacks |
| **Race Conditions** | [race-condition.md](race-condition.md) | Timing-based vulnerabilities and exploitation |
| **Parameter Pollution** | [parameter-pollution.md](parameter-pollution.md) | Parameter handling bypass techniques |
| **WAF Bypass** | [waf-bypass.md](waf-bypass.md) | Web Application Firewall evasion strategies |

### Special Topics

| Topic | File | Description |
|---|---|---|
| **Shellcode & Exploitation** | [shellcode.md](shellcode.md) | Shellcode development and payload techniques |
| **File Upload Vulnerabilities** | [file-upload.md](file-upload.md) | Upload validation bypass and exploitation |
| **Fuzzing Techniques** | [fuzzing.md](fuzzing.md) | Fuzzing methodologies for vulnerability discovery |
| **Fast Property Checking** | [fast-checking.md](fast-checking.md) | Rapid security assessment techniques |
| **OSINT (Open Source Intelligence)** | [osint.md](osint.md) | Information gathering and reconnaissance |
| **OSINT Methods** | [osint-method.md](osint-method.md) | Advanced OSINT methodologies |
| **GraphQL Security** | [graphql.md](graphql.md) | GraphQL-specific vulnerabilities and exploitation |
| **AI/LLM Pentesting** | [ai.md](ai.md) | AI and Large Language Model security vulnerabilities |

---

## 🎯 Getting Started

### Structure of Each Guide

Each markdown file follows a consistent structure for easy navigation:

1. **Shortcut** – Quick action items and high-level methodology
2. **Mechanisms** – Deep dive into how the vulnerability works
3. **Hunt** – Detailed hunting and discovery techniques
4. **Exploitation** – Step-by-step exploitation walkthroughs
5. **Impact** – Real-world impact assessment

### How to Use This Repository

1. **Identify the vulnerability type** you're interested in
2. **Read the "Shortcut" section** for the quick methodology
3. **Review the "Mechanisms" section** to understand how it works
4. **Follow the "Hunt" section** to discover vulnerabilities in target systems
5. **Use exploitation guides** to verify and exploit findings

### Example Usage

To investigate SQL Injection vulnerabilities:

1. Open `sql-injection.md` and read the `Shortcut` section to line up quick detection checks for the target endpoint.
2. Work through the `Mechanisms` and `Hunt` guidance to decide which payload families (boolean-based, time-based, stacked queries) make sense for the tech stack you're testing.
3. Use the payloads and tool suggestions in the `Exploitation` section while validating findings, then capture the potential business impact from the `Impact` notes for reporting.

To expand coverage during a web assessment:

1. Pivot to `xss.md`, `ssti.md`, or `file-upload.md` depending on the surface area you discover, following the same Shortcut → Mechanisms → Hunt flow.
2. Cross-reference `waf-bypass.md` when responses hint at defensive filtering.
3. Consult `progress.md` or your own testing worksheet to log which guides you have completed and identify remaining gaps.

For API or authentication reviews:

1. Start with `jwt.md`, `oauth.md`, or `graphql.md` to understand protocol-specific weaknesses before testing live traffic.
2. Combine reconnaissance tips from `osint.md` and `osint-method.md` with the authorization checks in `idor.md` to uncover privilege escalation paths.
3. If you uncover suspicious behavior, escalate to the advanced vectors in `req-smuggle.md` or `race-condition.md` to validate the full exploit chain.

---

## 🛠️ Tools & Resources

While this repository focuses on **methodologies and techniques**, common tools used alongside these guides include:

### Reconnaissance & Information Gathering
- Shodan, Censys (for asset discovery)
- amass, assetfinder (for subdomain enumeration)
- nmap, masscan (for port scanning)

### Web Application Testing
- Burp Suite (web proxy and scanner)
- OWASP ZAP (automated security scanning)
- Postman (API testing)

### Vulnerability-Specific Tools
- sqlmap (SQL injection)
- garak, LLMFuzzer (AI/LLM testing)
- nuclei (vulnerability scanning)
- ffuf, wfuzz (fuzzing)

---

## 💡 Use Cases

This repository is ideal for:

- 🔍 **Bug Bounty Hunters** – Discover vulnerabilities in web applications
- 🎓 **Security Students** – Learn penetration testing methodologies
- 🏢 **Penetration Testers** – Structure security assessments
- 🔒 **Security Researchers** – Reference for exploit development
- 📚 **Certification Prep** – Study for OSCP, GPEN, OWASP certifications

---

## 📖 Contributing

This is a community-driven project. Contributions are welcome!

To contribute:

1. **Fork the repository** and create a feature branch
2. **Add or improve documentation** with clear, practical examples
3. **Follow the existing structure** (Shortcut → Mechanisms → Hunt → Exploitation)
4. **Test your examples** and provide real-world context
5. **Submit a pull request** with a clear description

### Guidelines
- ✅ Use clear, concise language
- ✅ Include practical, tested examples
- ✅ Add tool recommendations where applicable
- ✅ Link to external resources and references
- ✅ Ensure payload examples are educational and ethical

---

## ⚠️ Disclaimer

This repository is provided for **educational and authorized security testing purposes only**.

- **Unauthorized access** to computer systems is illegal
- **Obtain proper authorization** before conducting security tests
- Use this knowledge **responsibly** and **ethically**
- The authors assume no liability for misuse of this information

---

## 📝 License

This project is provided as a community resource. Please check individual files for specific licensing information.

For questions or suggestions, feel free to open an issue or contribute to the project.

---

## 🤝 Credits

Built by the security community. Special thanks to all contributors who have shared their expertise and findings.

---

## 🔗 Quick Links

- **Security Standards**: [OWASP Top 10](https://owasp.org/www-project-top-ten/)
- **Learning Resources**: [PortSwigger Web Security Academy](https://portswigger.net/web-security)
- **Bug Bounties**: [HackerOne](https://www.hackerone.com/), [Bugcrowd](https://www.bugcrowd.com/)
