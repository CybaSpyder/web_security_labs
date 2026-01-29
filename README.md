# Web Security Labs

This repository documents hands-on web application security testing labs,
including SQL Injection, OWASP Top 10 vulnerabilities, and secure coding
mitigations using DVWA and Docker.

It is designed to demonstrate practical skills in:

- **Web Application Security (AppSec)**: Understanding common web vulnerabilities and their impact.
- **Vulnerability Assessment & Exploitation**: Identifying and safely testing security flaws in controlled lab environments.
- **Secure Coding Practices**: Implementing mitigations such as prepared statements, input validation, and proper error handling.
- **Containerized Lab Deployment**: Using Docker to create safe, reproducible environments for testing.
- **Security Reporting**: Documenting findings in professional, industry-standard reports.

---

## Repository Structure

```text
web-security-labs/
├── README.md                     # This file
├── security-reports/             # Formal assessment reports
│   ├── README.md
│   └── SQL-Injection-DVWA.md
├── labs/                         # Lab environments and notes
│   └── dvwa/
│       ├── setup.md
│       └── notes.md
└── docker/                       # Docker deployment files
    └── docker-compose.yml

```
## Security Reports

The `security-reports/` folder contains detailed security assessments conducted in controlled lab environments. Each report follows professional standards and includes:

- Vulnerability discovery process
- Exploitation steps
- Root cause analysis
- Risk assessment
- Remediation recommendations

**Example report:** [SQL Injection Assessment – DVWA](security-reports/SQL-Injection-DVWA.md)

## Labs

The `labs/` folder contains step-by-step instructions and notes for deploying the vulnerable web applications and practicing the security assessments.

Currently included:

- **DVWA (Damn Vulnerable Web Application)**: A deliberately insecure web app to practice OWASP Top 10 vulnerabilities.

## Docker Environment

All labs are containerized using Docker to ensure:

- Safe, isolated testing environments
- Reproducibility of experiments
- Easy setup for anyone cloning the repository

## Skills Demonstrated

Through these labs, the following professional skills are demonstrated:

- Web Application Security Testing (OWASP Top 10, DVWA)
- SQL Injection, XSS, CSRF testing
- Secure coding and mitigation strategies (Prepared Statements, Input Validation)
- Security reporting and documentation
- Containerized lab deployment using Docker
- Ethical hacking fundamentals in a controlled environment

## Getting Started

1. Install [Docker](https://www.docker.com/) on your machine
2. Clone this repository:

```bash
git clone https://github.com/CybaSpyder/web-security-labs.git
```
3. Navigate to the Docker folder and start the lab:

```bash
cd web-security-labs/docker
docker-compose up -d
```
4. Access DVWA in your browser:

```cpp
http://127.0.0.1
```
5. Follow the lab instructions in labs/dvwa/setup.md and explore the reports in security-reports/.\

---

## 6️⃣ License & Ethical Disclaimer

Very important for security labs:

```markdown
## License

This repository is for **educational purposes only**. All exercises are conducted in a safe, isolated lab environment. Do **not** attempt to test or exploit vulnerabilities on systems you do not own or have explicit permission to assess.


