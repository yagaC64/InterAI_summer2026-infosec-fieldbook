# Glossary

Student-friendly glossary for the InterAI Summer 2026 INFOSEC Fieldbook.

Security work has a ridiculous amount of acronym soup. Use this glossary to translate terms into plain English before writing findings, issues, pull requests, or review notes. If a term does not help the reader understand the risk or fix, do not use it just to sound official.

This is classroom vocabulary, not a formal compliance dictionary.

## How To Use This Glossary

- Use plain English first.
- Add the acronym only when it helps connect the finding to a known security practice.
- Do not claim formal compliance, certification, authorization, or audit results from a class review.
- If you find a secret, private data, or sensitive evidence, do not quote it publicly.

## Core Security Concepts

**AAA - Authentication, Authorization, and Accounting**  
Authentication asks "who are you?", authorization asks "what are you allowed to do?", and accounting records what happened.

**Access Control**  
Rules that decide who can view, change, run, or administer something. In student repos, this usually means checking whether admin paths, API keys, or write permissions are too open.

**Asset**  
Anything worth protecting: source code, data, accounts, API keys, build systems, websites, laptops, servers, cloud resources, or documentation.

**CIA Triad - Confidentiality, Integrity, Availability**  
The classic security model: keep private things private, keep data/code correct, and keep systems usable.

**Control**  
A safeguard or requirement that reduces risk. Examples include MFA, code review, dependency scanning, least privilege, backups, and logging.

**Finding**  
A specific issue discovered during review, with evidence, impact, and a suggested fix.

**Least Privilege**  
Give users, apps, and tokens only the access they need. No more. This is boring and powerful, which is the best kind of security.

**Risk**  
The chance that something bad could happen and the impact if it does. Do not call everything "critical"; that is how security language becomes noise.

**Threat**  
Something that could cause harm, such as an attacker, mistake, exposed token, broken dependency, or unsafe configuration.

**Vulnerability**  
A weakness that could be exploited or misused.

## Frameworks And Standards

**CIS Controls - Center for Internet Security Controls**  
Practical security safeguards used to organize cyber hygiene. In this fieldbook, CIS language is useful for basics like inventory, access control, secure configuration, and vulnerability management.

**CSF - Cybersecurity Framework**  
NIST's broad risk-management framework. CSF categories such as Govern, Identify, Protect, Detect, Respond, and Recover help organize security conversations without pretending a class review is a full audit.

**FIPS - Federal Information Processing Standards**  
Federal standards for certain security and technology requirements. Mention only when directly relevant; do not sprinkle it around like seasoning.

**FISMA - Federal Information Security Modernization Act**  
A US federal law governing information security programs for federal systems. Useful context for federal cybersecurity roles, but not something a student repo "passes" in class.

**FedRAMP - Federal Risk and Authorization Management Program**  
Federal authorization program for cloud products and services. Useful cloud-security vocabulary, but a class repo is not FedRAMP-authorized because someone used the word cloud.

**NIST - National Institute of Standards and Technology**  
US standards organization that publishes many cybersecurity references.

**NIST SP 800-53**  
NIST catalog of security and privacy controls. In this fieldbook, use it for vocabulary, not as a claim that a public class repo has been formally assessed.

**NIST SP 800-218 / SSDF - Secure Software Development Framework**  
NIST guidance for secure software development practices. This is a strong reference for class repo work because it connects security to how software is built.

**OWASP - Open Worldwide Application Security Project**  
Nonprofit security community known for practical application-security guidance.

**OWASP Top 10**  
Common categories of web application security risk. Use it to describe broad classes of problems, not to turn every small bug into a scary headline.

**RMF - Risk Management Framework**  
Federal process for categorizing systems, selecting controls, implementing controls, assessing controls, authorizing systems, and monitoring risk over time.

**Secure SDLC - Secure Software Development Life Cycle**  
Building security into planning, design, coding, testing, release, and maintenance.

## RMF, Authorization, And Evidence

**A&A - Assessment and Authorization**  
Process for assessing a system's security controls and deciding whether it can operate at an acceptable risk level.

**AO - Authorizing Official**  
Person with authority to accept risk and authorize system operation. In class, do not pretend to be the AO. Ay no, do not crown yourself.

**ATO - Authorization to Operate**  
Formal approval for a system to operate. A class review can support better security hygiene; it does not grant an ATO.

**C&A - Certification and Accreditation**  
Older term for what RMF-style Assessment and Authorization largely replaced. You may see it in older resumes or federal documents.

**CMAR - Continuous Monitoring Assessment Report**  
Report or artifact summarizing continuous monitoring status, findings, and posture. In class, a short review summary can borrow the idea without pretending to be a formal CMAR.

**ConMon / CONMON - Continuous Monitoring**  
Ongoing review of security posture, vulnerabilities, access, configuration, and risk.

**Control Assessment**  
Review of whether selected controls are implemented correctly and producing evidence.

**Control Evidence**  
Proof that a control exists and works, such as screenshots, configuration exports, logs, policy docs, scan reports, or test results. Public class evidence must not expose secrets or private data.

**IATT - Interim Authorization to Test**  
Temporary permission to test a system under controlled conditions. Do not use this term for normal student testing unless a real authorization process exists.

**DIACAP - DoD Information Assurance Certification and Accreditation Process**  
Older DoD authorization process largely replaced by RMF. You may see it in legacy resumes and documents.

**eMASS - Enterprise Mission Assurance Support Service**  
DoD system used to manage RMF packages, controls, artifacts, POA&Ms, and authorization workflow. Treat it as a federal GRC workflow reference, not a tool students need for class.

**Implementation Plan**  
Plan showing how security controls or remediation steps will be put in place.

**ISCM - Information Security Continuous Monitoring**  
Ongoing process for tracking security posture instead of treating security as a one-time event.

**POA&M / POAM - Plan of Action and Milestones**  
Tracking plan for known weaknesses, owners, milestones, and remediation status.

**Risk Acceptance**  
Decision to live with a known risk, usually because fixing it is not practical right now. Students should document risks clearly; they should not accept risk on behalf of someone else.

**SAR - Security Assessment Report**  
Report summarizing assessment results and findings. In class, your finding template is a lightweight cousin, not a formal SAR.

**SSP - System Security Plan**  
Document describing a system, its boundary, controls, environment, responsibilities, and security posture.

**ST&E - Security Test and Evaluation**  
Testing and evaluating security controls or system behavior.

**Xacta**  
Commercial GRC/RMF tool used to manage controls, artifacts, POA&Ms, and authorization workflows. Mention only as workflow vocabulary unless the actual tool is in scope.

## Federal Cyber Roles

**IA - Information Assurance**  
Older/common federal language for protecting information systems and ensuring confidentiality, integrity, availability, authentication, and non-repudiation.

**DoD 8570 / DoD 8140**  
DoD cybersecurity workforce qualification frameworks. Useful for understanding job categories and certification language, not for judging student repo quality.

**IAT - Information Assurance Technical**  
DoD workforce category for technical cybersecurity work.

**IAM - Information Assurance Management**  
DoD workforce category for cybersecurity management work.

**IASAE - Information Assurance System Architect and Engineer**  
DoD workforce category for higher-level security architecture and engineering work.

**ISSE - Information Systems Security Engineer**  
Security engineer focused on technical design, implementation, hardening, vulnerability management, and control engineering.

**ISSO - Information Systems Security Officer**  
Security officer focused on governance, evidence, controls, monitoring, access review, and risk tracking.

**ISSM - Information Systems Security Manager**  
Manager responsible for security program oversight, policy execution, and risk posture across systems or teams.

**SOC - Security Operations Center**  
Team or function that monitors alerts, investigates suspicious activity, and coordinates response.

## Vulnerability And Configuration Terms

**ACAS - Assured Compliance Assessment Solution**  
DoD vulnerability scanning and compliance ecosystem based around Tenable-style scanning. In class, use "vulnerability scanner" unless ACAS is specifically relevant.

**CVE - Common Vulnerabilities and Exposures**  
Public identifier for a known cybersecurity vulnerability.

**CVSS - Common Vulnerability Scoring System**  
Scoring system for vulnerability severity. Useful, but context still matters. A high CVSS score does not automatically mean a high class finding.

**CWE - Common Weakness Enumeration**  
Catalog of common software weakness types, such as injection or improper access control.

**DAST - Dynamic Application Security Testing**  
Testing a running application from the outside. Example: scanning a web app while it is live.

**SAST - Static Application Security Testing**  
Analyzing source code without running the app.

**SCA - Software Composition Analysis**  
Reviewing third-party dependencies for known vulnerabilities, licenses, or supply-chain risk.

**SBOM - Software Bill of Materials**  
Inventory of software components and dependencies. Helpful for understanding what a project depends on.

**SCAP - Security Content Automation Protocol**  
Standardized way to represent and automate security configuration and vulnerability checks.

**SRG - Security Requirements Guide**  
General security requirements for a technology or platform.

**STIG - Security Technical Implementation Guide**  
Detailed hardening guide. In class, do not say a repo is "STIG-compliant" unless a real STIG assessment happened.

**Vulnerability Management**  
Process of finding, prioritizing, fixing, and tracking vulnerabilities over time.

## Operations, Monitoring, And Incident Response

**Alert**  
Signal from a tool or system that something may need attention. Alerts are not automatically incidents.

**EDR - Endpoint Detection and Response**  
Tooling that monitors laptops, servers, or endpoints for suspicious behavior.

**Forensic Triage**  
Quick, careful review to decide what happened, what evidence exists, and what needs deeper investigation.

**IDS - Intrusion Detection System**  
Tool that detects suspicious network or system activity.

**IPS - Intrusion Prevention System**  
Tool that can block suspicious activity, not just detect it.

**IOC - Indicator of Compromise**  
Evidence that may suggest compromise, such as a malicious IP, hash, domain, file path, or behavior.

**IR - Incident Response**  
Process for handling a suspected or confirmed security incident.

**Log**  
Record of system, application, access, or security events.

**SIEM - Security Information and Event Management**  
Tool or platform that collects logs and events to support alerting, investigation, and reporting.

**SOAR - Security Orchestration, Automation, and Response**  
Automation that helps coordinate security response workflows.

**TTPs - Tactics, Techniques, and Procedures**  
How an adversary behaves. This term is useful when discussing patterns, not when describing every minor bug.

**XDR - Extended Detection and Response**  
Security platform that correlates activity across endpoints, identity, network, cloud, or other sources.

## Identity, Access, And Accounts

**ABAC - Attribute-Based Access Control**  
Access decisions based on attributes such as department, role, project, device state, or location.

**ACL - Access Control List**  
List defining who can access a resource and what actions they can perform.

**IAM - Identity and Access Management**  
Tools and processes for users, roles, authentication, and permissions. Also used as a DoD workforce acronym; context matters.

**ICAM - Identity, Credential, and Access Management**  
Federal identity/access language covering identity proofing, credentials, authentication, authorization, and account lifecycle.

**MFA - Multi-Factor Authentication**  
Authentication using more than one factor, such as password plus app prompt, hardware key, or code.

**PAM - Privileged Access Management**  
Controls for administrator or high-risk accounts.

**RBAC - Role-Based Access Control**  
Access based on assigned roles, such as student, maintainer, reviewer, or admin.

**SAAR - System Authorization Access Request**  
Formal access request process, often seen in federal environments.

**SSO - Single Sign-On**  
Using one identity provider to sign into multiple services.

## System Boundaries And Architecture

**API - Application Programming Interface**  
Interface that lets software talk to other software.

**Authorization Boundary**  
The system components, users, data flows, and responsibilities included in a security assessment.

**Boundary Diagram**  
Visual showing what is inside and outside the system boundary.

**Data Flow**  
How data moves through a system, including inputs, outputs, storage, and third-party services.

**PPS - Ports, Protocols, and Services**  
Network communication details. Useful for system reviews, but usually too deep for a basic static class repo.

**PPSM - Ports, Protocols, and Services Management**  
Process for managing and approving network ports, protocols, and services.

**System Owner**  
Person or group responsible for a system's operation and risk.

**Zero Trust**  
Security model that avoids assuming trust just because something is inside a network. It usually involves identity, device posture, least privilege, segmentation, and continuous validation.

## Resilience And Recovery

**BCP - Business Continuity Plan**  
Plan for keeping important functions running during disruption.

**Backup**  
Copy of data or systems that can be restored after deletion, corruption, or failure.

**COOP - Continuity of Operations**  
Planning for continuing mission or business operations during disruption.

**DR - Disaster Recovery**  
Restoring systems and data after major failure or incident.

**RTO - Recovery Time Objective**  
How quickly a system needs to be restored.

**RPO - Recovery Point Objective**  
How much data loss is acceptable, measured by time since the last recoverable backup.

## Class Repo Review Terms

**Dependency Hygiene**  
Keeping dependency files clear, reproducible, and reasonably current.

**Evidence Handling**  
Collecting and describing proof without leaking sensitive data.

**False Positive**  
A tool reports a problem that is not actually a problem in context.

**Public-Safe Finding**  
A finding that explains the issue without exposing secrets, personal data, or exploit details.

**Reproducibility**  
Whether someone else can build, run, or verify the project from the repo instructions.

**Scanner Noise**  
Raw tool output that produces lots of alerts without useful explanation or prioritization.

**Secret**  
Any credential-like value that could grant access: API key, token, password, private key, webhook secret, session cookie, or certificate material.

**Sensitive Data**  
Information that should not be public, including private contact info, grades, identity mapping, credentials, personal data, private screenshots, or operational details.

**Small PR**  
A pull request that fixes one clear thing and is easy to review. This is usually better than a heroic rewrite. Heroics are how bugs wear a cape.

## Acronyms Students Should Be Careful With

These terms are real, but easy to overclaim:

- **ATO**: Do not say a class repo has one.
- **Compliance**: Say "aligned with" or "inspired by" unless a formal assessment exists.
- **Critical**: Reserve for issues with clear, serious impact.
- **Exploit**: Avoid exploit instructions in public class work.
- **FISMA / FedRAMP / RMF**: Useful vocabulary, not classroom certification badges.
- **STIG-compliant**: Only say this after a real STIG assessment.

## Plain-English Translation Pattern

When writing findings, use this pattern:

```text
Instead of: "The repository has poor access-control hygiene."

Say: "The app has an admin-looking route, but the README does not explain whether it is protected. Please document the expected access control or add a small guard so non-admin users cannot reach it."
```

```text
Instead of: "This violates secure SDLC."

Say: "The project depends on packages, but there is no lockfile or setup note. Adding reproducible install instructions would make the project easier to review and safer to maintain."
```
