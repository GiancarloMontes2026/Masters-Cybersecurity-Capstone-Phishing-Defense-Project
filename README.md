# Layered Email Security & Phishing Defense Implementation

## Overview

This project documents my cybersecurity capstone focused on designing and implementing a defense-in-depth security solution for a fictional organization, Yummy Pretzel Co.

The project addresses a successful phishing attack in which a malicious email attachment resulted in malware execution, command-and-control (C2) communication, unauthorized access, and the exfiltration of proprietary business information and employee Personally Identifiable Information (PII).

The objective was to determine the root causes of the compromise and design a layered cybersecurity solution capable of preventing, detecting, containing, and responding to similar attacks.

## Incident Scenario

The simulated incident began when an employee received a phishing email impersonating a legitimate company. The message contained a malicious attachment that was opened by the employee.

After execution, the malware established communication with external command-and-control infrastructure. The attacker subsequently gained unauthorized access to internal resources and exfiltrated sensitive business information and employee PII.

The investigation identified several contributing security weaknesses:

- Insufficient email authentication
- Inadequate malicious email and attachment filtering
- Endpoint protection limitations
- Excessive reliance on employee judgment
- Insufficient defense-in-depth

## Security Solution

The proposed architecture uses multiple security layers to reduce the likelihood that a single successful phishing interaction can result in a larger compromise.

### Email Security

Email protections include:

- SPF
- DKIM
- DMARC
- S/MIME
- Secure email filtering
- Malicious attachment detection
- Malicious URL detection
- Email quarantine policies

These controls are designed to reduce email spoofing, detect malicious content, protect email communications, and prevent phishing messages from reaching users.

### Endpoint Security

Microsoft Defender for Endpoint provides Endpoint Detection and Response (EDR) capabilities for:

- Malware detection
- Endpoint monitoring
- Security investigation
- Device isolation

Endpoint protection provides another defensive layer if malicious content successfully reaches and executes on a workstation.

### Identity & Access Management

Microsoft Entra ID and Multi-Factor Authentication (MFA) are incorporated to reduce the risk of unauthorized access when credentials are compromised.

Identity protections include:

- MFA
- Conditional Access
- Authentication monitoring
- Least-privilege principles
- Access controls

### Security Awareness

The technical controls are supplemented with employee cybersecurity awareness training and simulated phishing campaigns.

Training focuses on:

- Identifying phishing emails
- Recognizing suspicious links and attachments
- Verifying unexpected requests
- Reporting suspicious messages
- Protecting sensitive information
- Reporting suspected malware infections

## Cybersecurity Frameworks

The project uses the NIST Cybersecurity Framework (CSF) 2.0 as its primary risk-management framework.

Security activities are organized around:

**Govern → Identify → Protect → Detect → Respond → Recover**

NIST SP 800-53 is also used to support the selection of security and privacy controls related to access control, authentication, auditing, incident response, communications protection, and system integrity.

NIST incident response guidance is incorporated into the detection, response, containment, and recovery portions of the project.

## Implementation Strategy

The project follows a phased Waterfall implementation methodology:

1. Project Initiation & Planning
2. Security Assessment & Baseline Development
3. Solution Design & Configuration
4. Pilot Implementation
5. Production Rollout
6. Validation & Security Testing
7. Project Closure & Transition to Operations

Controls are initially configured and validated in a controlled environment before pilot deployment and organization-wide implementation.

This approach reduces the risk of security-control misconfiguration and business disruption.

## Risk Assessment

Implementation risks evaluated during the project include:

- Security-control misconfiguration
- Compatibility and interoperability problems
- Disruption to legitimate email
- Employee resistance
- Insufficient pre-production testing
- S/MIME certificate deployment issues
- Resource and budget constraints
- Implementation delays

Each risk was evaluated according to its likelihood, potential impact, and appropriate mitigation strategy.

## Security Testing & Validation

The security architecture is validated through controlled technical testing and phishing simulations.

Testing includes:

- Spoofed email detection
- SPF/DKIM/DMARC validation
- Malicious attachment detection
- Email filtering
- EDR malware detection
- Endpoint isolation
- MFA authentication
- S/MIME functionality
- Security alert generation
- Controlled phishing simulations

The final testing scenario recreates the original attack chain:

**Phishing Email → Malicious Attachment → Endpoint Execution → Malware Detection → Endpoint Isolation → Incident Alert**

The objective is to determine whether the implemented security controls can prevent the simulated attack from progressing through the same stages as the original incident.

## Security Metrics & KPIs

The project establishes measurable security objectives, including:

- ≥95% malicious email detection
- ≥95% malicious attachment detection
- 100% test-malware detection by EDR
- Endpoint isolation within 5 minutes
- 100% MFA enrollment
- 100% SPF/DKIM/DMARC configuration
- Zero critical unresolved implementation vulnerabilities
- ≤5% successful phishing simulation rate
- ≥80% phishing reporting rate
- Zero critical business-disruption incidents

These metrics provide measurable criteria for determining whether the security implementation successfully reduces organizational risk.

## Tools & Technologies

- Microsoft Defender for Office 365
- Microsoft Defender for Endpoint
- Microsoft Entra ID
- Multi-Factor Authentication (MFA)
- Conditional Access
- S/MIME
- SPF
- DKIM
- DMARC
- Endpoint Detection & Response (EDR)
- Microsoft 365
- KnowBe4
- Centralized Security Logging & Monitoring
- Vulnerability Scanning

## Frameworks & Standards

- NIST Cybersecurity Framework 2.0
- NIST SP 800-53
- NIST Incident Response Guidance
- NIST Phish Scale

## Skills Demonstrated

**Phishing Defense • Security Architecture • Defense-in-Depth • Email Security • Endpoint Security • EDR • IAM • MFA • Incident Response • Risk Assessment • Security Controls • Security Awareness • Security Monitoring • Security Testing • Vulnerability Management • Technical Documentation • Project Management • NIST CSF**

## Project Deliverables

The project produced or planned several cybersecurity deliverables:

- Security Assessment Report
- Technical Solution Design
- Implementation Documentation
- Testing & Validation Report
- Security Awareness Training Materials
- Project Risk Register
- Final Cybersecurity Project Report

## Key Takeaways

This project demonstrates how a phishing incident can be addressed through a layered security strategy rather than relying on a single security product or employee awareness alone.

The solution combines email authentication, secure email technologies, endpoint detection and response, identity protection, centralized monitoring, incident response, security awareness, risk management, and measurable security testing.

The project strengthened my experience translating an identified cybersecurity risk into technical controls, implementation requirements, testing procedures, risk mitigation strategies, security metrics, documentation, and operational recommendations.

## Disclaimer

Yummy Pretzel Co. is a fictional organization created for an academic cybersecurity project. The attack scenario, organizational data, implementation plan, and testing activities were developed for educational purposes. No production systems or real organizational data were used.
