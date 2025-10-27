

# 🧩 Common Vulnerabilities and Exposures (CVE)

and

# 🧰 Common Weakness Enumeration (CWE)

---

## 🔹 **1. Common Vulnerabilities and Exposures (CVE)**

### 📘 **Definition:**

CVE is a **publicly available list of known cybersecurity vulnerabilities** in software and hardware systems.
Each CVE entry contains a **unique ID**, a **brief description**, and **references** to additional details and patches.

CVE helps organizations and researchers speak a **common language** when discussing security flaws.

---

### 🧩 **Structure of a CVE ID:**

Example: `CVE-2021-44228`

* **CVE:** Common Vulnerabilities and Exposures
* **2021:** Year the vulnerability was published
* **44228:** Unique identifier number

This example refers to the **Log4Shell** vulnerability in Apache Log4j, one of the most critical flaws discovered in 2021.

---

### ⚙️ **CVE Entry Components:**

* **CVE ID** – Unique identifier for each vulnerability
* **Description** – Short explanation of the issue
* **References** – Links to patches, advisories, or research papers
* **CVSS Score** – Indicates severity (0.0–10.0)

  * 0.1–3.9 → Low
  * 4.0–6.9 → Medium
  * 7.0–8.9 → High
  * 9.0–10.0 → Critical

---

### 🧠 **Purpose of CVE:**

* Provides a **standardized naming system** for vulnerabilities
* Helps **security tools** (like Nessus, OpenVAS, Metasploit) align detection results
* Enables faster **communication and patching** among organizations

---

### 🧪 **Practical Use Case:**

A security analyst scans a network with a vulnerability scanner.
The tool reports:

> "Vulnerability Detected: CVE-2021-34527 (PrintNightmare)."

This allows the analyst to quickly:

1. Search the CVE database
2. Understand the risk level
3. Apply official mitigation or patch

---

## 🔹 **2. Common Weakness Enumeration (CWE)**

### 📘 **Definition:**

CWE is a **catalog of software and hardware weakness types** that lead to vulnerabilities.
It focuses on the **root causes** of vulnerabilities rather than specific instances.

If **CVE** is a *specific security hole*, then **CWE** describes the *category or pattern* of the mistake that caused it.

---

### 🧩 **Example Mapping:**

| CVE ID         | CWE ID  | Description                       |
| -------------- | ------- | --------------------------------- |
| CVE-2021-44228 | CWE-502 | Deserialization of Untrusted Data |
| CVE-2017-5638  | CWE-78  | OS Command Injection              |
| CVE-2020-0601  | CWE-295 | Improper Certificate Validation   |

---

### ⚙️ **Common CWE Categories:**

| CWE ID      | Weakness Name                     | Description                                    |
| ----------- | --------------------------------- | ---------------------------------------------- |
| **CWE-79**  | Cross-Site Scripting (XSS)        | Injection of malicious JavaScript              |
| **CWE-89**  | SQL Injection                     | Manipulating SQL queries via input             |
| **CWE-20**  | Improper Input Validation         | Failing to check user inputs                   |
| **CWE-119** | Buffer Overflow                   | Writing outside memory bounds                  |
| **CWE-352** | Cross-Site Request Forgery (CSRF) | Forcing user actions in authenticated sessions |

---

### 🧠 **Purpose of CWE:**

* Guides **developers** to write secure code
* Helps **security testers** identify recurring patterns of weaknesses
* Supports **researchers** in classifying vulnerabilities
* Assists **organizations** in reducing common software flaws

---

## 🔄 **Relationship Between CVE and CWE**

| Aspect            | CVE                                           | CWE                                     |
| ----------------- | --------------------------------------------- | --------------------------------------- |
| **Focus**         | Specific vulnerability instance               | General weakness type                   |
| **Purpose**       | Identify and track known vulnerabilities      | Describe common coding and design flaws |
| **Maintained by** | MITRE                                         | MITRE                                   |
| **Used by**       | Security Analysts, Tools, Incident Responders | Developers, Researchers                 |
| **Example**       | CVE-2021-44228 (Log4Shell)                    | CWE-502 (Deserialization flaw)          |

---


