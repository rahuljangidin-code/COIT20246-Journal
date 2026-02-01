# Week 09 – Attacks and Vulnerabilities

---

## Task 1 – Knowledge Test

The Week 09 knowledge test was completed during the tutorial as required.

---

## Task 2 – CIA Asset Identification

The important assets for the project were identified and analysed using the CIA Triad.

### Asset List and CIA Protection

| Asset | Protection | Reason |
|------|-----------|--------|
| Customer personal data | Confidentiality | Customer data must be protected to prevent unauthorised access and privacy breaches. |
| Application server | Availability | The server must remain operational to ensure services are continuously accessible. |
| Network configuration files | Integrity | Configuration files must not be altered without authorisation as this could cause system failure. |
| Backup data | Availability | Backups are required to restore systems after failures or attacks. |
| User authentication credentials | Confidentiality | Credentials must be protected to prevent account compromise. |

---

## Task 3 – Threat Sources and Motivation

Potential threat sources and their motivations were identified for the project environment.

### Threat Source List

| Threat Source | Motivation |
|-------------|-----------|
| External hacker | To gain unauthorised access to systems or steal sensitive data. |
| Insider employee | Misuse of access for personal gain or due to negligence. |
| Competitor organisation | To disrupt services or gain competitive advantage. |
| Malware developer | To distribute malicious software for financial or reputational gain. |

---

## Task 4 – Vulnerability Analysis (CVEs)

Three vulnerabilities with different severity levels were analysed using the NIST National Vulnerability Database.

---

### CVE 1 – Critical Severity

| Category | Details |
|--------|--------|
| CVE ID | CVE-2023-34362 |
| Description | A remote code execution vulnerability affecting MOVEit Transfer software. |
| CVSS Score | 9.8 (Critical) |
| CIA Impact | Confidentiality: High, Integrity: High, Availability: High |
| CWE | CWE-502 – Deserialization of Untrusted Data |
| Company | Progress Software |
| Product | MOVEit Transfer |
| Mitigation | Apply vendor security patches and restrict external access. |
| Simple Explanation | This vulnerability allows attackers to run malicious code remotely, giving them full control over the system. |

---

### CVE 2 – High Severity

| Category | Details |
|--------|--------|
| CVE ID | CVE-2022-22965 |
| Description | A remote code execution vulnerability in Spring Framework. |
| CVSS Score | 9.0 (High) |
| CIA Impact | Confidentiality: High, Integrity: High, Availability: Medium |
| CWE | CWE-94 – Improper Control of Code Generation |
| Company | VMware |
| Product | Spring Framework |
| Mitigation | Update to patched versions and restrict exposed services. |
| Simple Explanation | The flaw allows attackers to inject and execute code by sending crafted requests to the application. |

---

### CVE 3 – Medium Severity

| Category | Details |
|--------|--------|
| CVE ID | CVE-2021-3449 |
| Description | A denial-of-service vulnerability in OpenSSL. |
| CVSS Score | 5.9 (Medium) |
| CIA Impact | Confidentiality: Low, Integrity: Low, Availability: Medium |
| CWE | CWE-400 – Uncontrolled Resource Consumption |
| Company | OpenSSL Project |
| Product | OpenSSL |
| Mitigation | Update OpenSSL and monitor resource usage. |
| Simple Explanation | This vulnerability allows attackers to consume system resources, causing service disruption. |

---

## Task 5 – Vulnerability Disclosure

Vulnerability disclosure involves balancing security and transparency. Vendors may delay public disclosure to allow time for patch development and testing. This helps reduce the risk of attackers exploiting the vulnerability before a fix is available.

A reasonable disclosure period allows vendors to prepare mitigation measures while keeping users informed. If vulnerabilities are disclosed too early, systems may be exposed without protection. However, excessive delays reduce trust and increase risk.

Responsible disclosure ensures cooperation between researchers and vendors. It protects users while maintaining ethical standards in cybersecurity.
