# PatchGuard
OT/ICS Vulnerability Management Platform# PatchGuard - OT/ICS Vulnerability Management Platform

![PatchGuard](https://img.shields.io/badge/version-0.1.0-blue)
![License](https://img.shields.io/badge/license-MIT-green)
![Python](https://img.shields.io/badge/python-3.9+-blue)

**PatchGuard** is an open-source vulnerability management platform designed for **OT/ICS environments** in oil & gas, utilities, manufacturing, and critical infrastructure.

## What It Does

**Phase 1 (MVP):**
- ✅ Discover installed software (Windows & Linux)
- ✅ Send inventory to centralized server
- ✅ Check against NVD (National Vulnerability Database)
- ✅ Display vulnerabilities in web dashboard
- ✅ Alert on critical/high-risk issues

**Future Phases (v1.5+):**
- Automated patching with approval workflows
- Multi-site management
- Compliance reporting (NERC CIP, NIST SP 800-82)
- AI-powered risk scoring

## Quick Start

### Prerequisites
- Python 3.9+
- Windows / Linux / macOS

### Installation

```bash
# Clone
git clone https://github.com/OTBn/patchguard.git
cd patchguard

# Install
pip install -r requirements.txt

# Terminal 1: Start server
python -m uvicorn server.api:app --reload

# Terminal 2: Run agent
python agent/scanner.py

# Open browser
http://localhost:8000/dashboard
