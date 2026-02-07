## Components and roles

- Mobile app
  - Programmer (Mobile)
  - QA
- 3rd party bot services
  - Volunteers
- SMS providers
  - 3rd party provider companies
- Message handling service
  - Backend programmer
  - QA
- AUTH & Session service
  - Backend programmer
  - QA
  - Cybersec engineer

## Roles and responsibilities

- Programmer (Mobile) - Designs and builds the mobile app screens and features, integrating APIs, local storage, and device capabilities so users can register, receive SMS, and interact smoothly with the service. They also fix bugs, improve performance on different phones, and keep the app updated with OS changes.
- Backend programmer – Implements server‑side logic for the message handling and AUTH & Session services, including APIs, database models, and message routing workflows. They ensure secure data processing, authorization checks, and performance/scalability under high traffic.
- QA (Quality Assurance) – Plans and executes manual and automated tests across the mobile app and backend services to catch defects before release. They verify that requirements are met, regressions are avoided, and edge cases (failed SMS, expired sessions, etc.) behave correctly.
- Cybersec engineer – Focuses on securing the AUTH & Session and message handling services by doing threat modeling, vulnerability assessments, and code reviews with a security lens. They define and enforce encryption, authentication, and authorization practices, monitor for attacks, and ensure compliance with relevant security standards.
- Volunteers (3rd party bot services) – Configure and operate chatbots or support flows that interact with users via external platforms, making sure messages are correctly formatted and routed into your system. They also report issues, help refine conversation scripts, and coordinate with developers when integrations break or new scenarios are needed.

## Common skills across these roles

- Programmer (Mobile)
  - Programming in Swift/Kotlin or cross‑platform frameworks, API integration, and basic database work.
  - Understanding of UI/UX principles, debugging, and performance optimization on mobile devices.
- Backend programmer
  - Server‑side languages (for example Python, Java, Node.js), web frameworks, and REST API design.
  - Database management (SQL/NoSQL), security basics, and deployment/version‑control tools.
- QA
  - Test case design, manual and automated testing, and bug tracking tools.
  - Basic understanding of SDLC, API and cross‑platform testing, and clear communication of defects.
- Cybersec engineer
  - Network security, cryptography, vulnerability assessment, and incident response skills.
  - Knowledge of penetration testing tools, firewalls/SIEM, and secure configuration of systems.
- Volunteers (3rd party bot services)
  - Basic technical literacy with chat platforms or bots and ability to follow integration/runbooks.
  - Soft skills like communication, reliability, and organization when coordinating with the core team.

## My chosen role

Cybersecurity specialist (Junior / SOC Analyst L1 direction).

Skills I already have
- Programming basics in C/C++ (I can write and debug code; I’m used to algorithmic problem-solving).
- Command line workflow + development tooling (terminal usage, compile/run locally, VS Code).
- Git basics (creating repos, configuring `.gitignore`, using Git from terminal).
- Core CS foundations (data structures like linked lists; complexity/algorithms mindset helps for log/alert triage thinking).
- Basic awareness of security role responsibilities (network security, vulnerability assessment, incident response as the “shape” of the job). [cite:7]  

Skills I lack
- SIEM/log analysis practice (working with syslog/event logs/netflow, building investigation habits).
- Networking and traffic analysis tools in practice (e.g., tcpdump/Wireshark, common troubleshooting commands).
- Vulnerability management & threat hunting fundamentals as real workflows (triage, prioritization, documenting findings).
- Operating system hardening (Windows/*nix permissions, secure configuration, patching, isolation concepts).
- Incident response “runbooks” + reporting discipline (procedures, escalation, false positive/false negative handling).

---

Job postings (5–7)

Posting 1
- **Role title:** Junior ИБ специалист  
- **Link:** https://hh.ru/vacancy/129647623
- **Key skills/requirements (3–5):**
- PKI/cryptography concepts (certificates, keys) and security requirements/risk thinking.
- Scripting/automation basics; working with data and SQL queries/dashboards.
- OS setup skills + network security basics; monitoring tooling (mentions Zabbix/Grafana) and SNMP.

Posting 2
- **Role title:** SOC Analyst (L1 / Junior Cybersecurity Analyst)  
- **Link:** https://dreamjob.ru/employers/107846/vakansii/128996189
- **Key skills/requirements (3–5):**
- Monitoring security events in SIEM; working with alerts.
- первичный анализ (L1) + escalation to next level; ticketing/reporting.
- Understanding of networks, logs, and common attack ideas; English ≥ Intermediate.

Posting 3
- **Role title:** Специалист отдела информационной безопасности (Junior)  
- **Link:** https://dreamjob.ru/employers/129225/vakansii/128940889
- **Key skills/requirements (3–5):**
- Basic security management tasks (controls for provider/clients; personal data security).
- Understanding typical attacks/vulnerabilities and ability to search for vulnerabilities manually.
- Knowledge of regulatory/legal base (documentation, compliance/attestation support).

Posting 4
- **Role title:** Специалист по информационной безопасности (mid+ example)  
- **Link:** https://career.habr.com/vacancies/1000148301
- **Key skills/requirements (3–5):**
- Administering security systems; incident management end-to-end.
- OS security knowledge (Windows, *nix, macOS) + strong networking/virtualization knowledge.
- Log analysis; automation/optimization of security management.

Posting 5
- **Role title:** Cyber Security Expert roadmap (skills list reference)  
- **Link:** https://roadmap.sh/cyber-security
- **Key skills/requirements (3–5) “implied by roadmap”:**
- Operating systems (Windows/Linux/macOS), permissions, troubleshooting.
- Networking knowledge + tooling (nmap/tcpdump etc.).
- Detection/defense concepts (IDS/IPS, hardening, logs).

---

Job market snapshot

Skills that appear in several postings
- Log/alert monitoring + reporting/ticketing mindset (SOC/SIEM, “analyze events”, write up results).  
- Networking fundamentals and ability to reason about attacks/traffic/logs.  
- OS/security administration basics (Windows/*nix; secure configuration expectations).
- Automation/scripting + working with data (SQL/dashboards/automation mentioned as valuable).

Skills specific to a single posting
- PKI/cryptography for payment systems + certificate/key workflows (very domain-specific).  
- SNMP/RedOS + Zabbix/Grafana monitoring stack specific tooling combination.
- Regulatory/compliance documentation and attestation support (more “governance” flavor).  
- Virtualization “deep knowledge” as a highlighted requirement (strong in the Habr posting).

---

Personal reflection (5–10 sentences)

I chose the **cybersecurity specialist** path, leaning toward SOC / incident response, because it combines technical problem-solving with real-world impact: detecting attacks, analyzing evidence, and improving defenses.
Compared to market expectations, my strongest overlap is general engineering discipline: I can program in C/C++, I’m comfortable working in a terminal/IDE workflow, and I use Git—these help with automation and structured investigations.  
The biggest gap is that job postings and the roadmap emphasize operational security work: SIEM/log analysis, networking visibility, and repeatable incident-response procedures, which I haven’t practiced as “daily workflow” yet.
This semester I want to develop (1) **network traffic + log analysis** (tcpdump/Wireshark basics, understanding common protocols, reading syslog/event logs) because it appears across SOC-style roles and directly affects my ability to triage alerts.
Second, I want to build (2) a small incident-response “mini-lab” habit (write simple runbooks, document false positives, practice escalation notes) because postings explicitly care about process, reporting, and incident handling—not only theory.
If I do these two things, my existing coding skills should start translating into security automation and better investigation quality, which aligns with what employers mention (automation + incident management).