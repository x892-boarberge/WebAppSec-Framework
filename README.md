# WebAppSec Framework

**An Evidence-Based, Risk-Prioritised Web Application Security Improvement Framework**

## 🌐 Live Demo
You do not need to install any software to view this project. 
👉 **[Click here to view the live dashboard](https://x892-boarberge.github.io/WebAppSec-Framework/)**

## ✨ Key Features
*   **Interactive Dashboard:** Click on any metric (e.g., "Critical Risk") to instantly portal to a filtered register of those specific vulnerabilities.
*   **Fully Mobile Responsive:** Designed with touch targets, 2x2 metric grids, and horizontally scrolling tables to accommodate iOS and Android devices perfectly.
*   **Evidence-Based Data:** Every vulnerability is triangulated with OWASP/NIST standards and peer-reviewed academic papers.
*   **Four-Layer Framework:** Maps each vulnerability to Prevent, Detect, Respond, and Verify controls.

## Overview
This repository contains the artefact and research documentation for a BSc (Hons) Cyber Security dissertation. The project investigates common web application vulnerabilities, assesses their risk using a structured 5×5 likelihood-impact matrix, and maps them to a four-layer security improvement framework.

## Project Structure
*   data/ - Contains the ulnerabilities.json source of truth (12 assessed vulnerabilities).
*   docs/ - Contains methodology notes, traceability matrices, and the dissertation chapters.
*   prototype/ - Contains the static HTML/CSS/JS web application.
*   	ests/ - Contains functional test reports (T01-T08) and screenshot evidence.

## How to Run Locally (Optional)
If you wish to run the prototype on your own machine (e.g., to edit the code), you cannot simply double-click index.html because browsers block etch() requests on local files for security reasons (CORS). 

You must serve the files via a local server:
1. Open your terminal in the root of this project.
2. Run: \python -m http.server 8000\
3. Open your browser and navigate to: \http://localhost:8000/prototype/index.html\

## Framework Overview
The project utilises a four-layer control mapping model, drawing from industry standards:
*   **Prevent:** OWASP Cheat Sheets
*   **Detect:** OWASP WSTG (or documented gaps)
*   **Respond:** NIST CSF 2.0
*   **Verify:** OWASP ASVS 5.0.0
