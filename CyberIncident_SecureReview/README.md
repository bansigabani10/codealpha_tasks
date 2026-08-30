# 🔐 CyberIncident — Secure Coding Review & Incident Management System

A Flask-based cybersecurity application designed to demonstrate **secure coding practices, cyber incident reporting, automated incident workflow, security analysis, and SOC-oriented incident management**.

This project was developed as a practical cybersecurity project to understand how secure web applications can support the reporting, analysis, tracking, and investigation of security incidents.

---

## 📌 Project Overview

Cyber incidents such as phishing, malware infections, ransomware, account compromise, data breaches, and network intrusions require structured reporting and investigation.

This project provides a web-based platform where users can:

- Create an account
- Log in securely
- Report cybersecurity incidents
- Provide incident details
- Track incident progress
- Review security-related information
- Follow an automated investigation workflow

The application also demonstrates how automated processing can prepare an incident for further **SOC analyst review**.

---

# 🎯 Objectives

The main objectives of this project are:

- Build a practical cybersecurity web application
- Apply secure coding principles
- Implement authentication and password protection
- Provide structured cyber incident reporting
- Store incident information using a database
- Automate initial incident workflow processing
- Identify IP address indicators from incident reports
- Create investigation timelines
- Prepare incidents for analyst review
- Document security considerations and improvements

---

# 🚀 Key Features

## 🔑 1. User Authentication

The application provides:

- User registration
- User login
- Session management
- Password verification
- Password hashing

Passwords are processed using Werkzeug password-hashing utilities rather than being stored as plain text.

---

## 🚨 2. Cyber Incident Reporting

Users can report cybersecurity incidents through a structured form.

The system supports incident categories such as:

- Phishing Email
- Malware Infection
- Ransomware Attack
- Data Breach
- Account Hacking
- Website Defacement
- Network Intrusion
- Suspicious Activity

Each incident can contain relevant information such as:

- Incident title
- Description
- Incident type
- Severity
- Related indicators

---

# 🔍 3. Automated Incident Workflow

After an incident is reported, the application creates an investigation workflow based on the incident type.

For example, a phishing incident can progress through:

```text
Reported
    ↓
Investigation Queued
    ↓
Email Analysis
    ↓
Sender Analysis
    ↓
URL Analysis
    ↓
IP Reputation Check
    ↓
User Activity Check
    ↓
Threat Assessment
    ↓
Analyst Review Required
