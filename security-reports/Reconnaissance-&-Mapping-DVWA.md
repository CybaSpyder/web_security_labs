# 🔍 DVWA Forensics Report  
## Phase 1: Reconnaissance & Attack Surface Mapping

---

## 📌 Overview

This report documents the full **Reconnaissance & Mapping** of a controlled security assessment performed against **Damn Vulnerable Web Application (DVWA)** in a local lab environment.

The purpose of this phase is to **identify and enumerate all user-controlled input vectors within DVWA** and understand how data is transmitted from client to server.

> ⚠️ No exploitation was performed during this phase.

This reconnaissance phase establishes the foundation for all subsequent vulnerability testing and exploitation.

---

## 🎯 Objective

To Create a complete list of every location where user input enters DVWA and how it is transmitted to the server.

### Specific Goals

- Identify all DVWA modules that accept user input  
- Capture request structure (URL, HTTP method, parameters)  
- Determine input types and controllability  
- Establish a complete attack surface map for later phases  

---

## 🧪 Environment Details

| Component | Details |
|-----------|----------|
| Application | Damn Vulnerable Web Application (DVWA) |
| Deployment | Localhost |
| Web Server | Apache |
| Backend | PHP / MySQL |
| DVWA Security Level | Low |
| Authentication | `admin / password` |
| Interception Tool | Burp Suite (Proxy) |
| Browser | Burp Built-in Chromium |

---

## 🛠 Tools Used

- **Burp Suite (Community Edition)**  
  - Proxy  
  - HTTP History  
- Web Browser (via Burp)  
- DVWA Source Code (View Source)
<img width="1596" height="896" alt="Burp3" src="https://github.com/user-attachments/assets/6d0cdebe-f319-4baa-ac3c-a4f075711dcc" />
  Burp Suite set-up.

---

## ⚙️ Methodology

The reconnaissance process followed a **manual and systematic penetration testing workflow**:

1. DVWA security level set to **Low** to observe unprotected behavior  
2. Browser traffic routed through **Burp Suite Proxy**  
3. Each DVWA vulnerability module accessed sequentially  
4. Forms, links, and parameters submitted with benign test input  
5. HTTP requests captured and analyzed in Burp  
6. User-controlled parameters documented without exploitation  

> ⚠️ No payloads, injections, or attack techniques were used in this phase.

---

## 🔎 Attack Surface Mapping

All identified user inputs were documented in a structured **Attack Surface Table**, capturing:

- DVWA module name  
- Endpoint URL  
- Input field names  
- Input types  
- HTTP methods  
- Parameters sent to the server  
- Initial security observations  

---

## 📎 Attack Surface Table

> **External Reference (Google Sheets)**  
> <a href="https://docs.google.com/spreadsheets/d/1NmwNs2hRue8znp7cgOQM6khAKIg7oZ9WcCET4n-HSbM/edit?usp=sharing">Recon Results Table<a/>

