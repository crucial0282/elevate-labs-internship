# 🔍 Nessus Vulnerability Scan Report
## 🧪 Scan Overview

    Tool Used: Tenable Nessus

    Scan Type: Basic Network Vulnerability Scan

    Targets Scanned: 2 hosts

    File Format: .nessus (XML-based export)

    Report Included: Summary PDF (see Nessus_Scan_Report_Summary.pdf)

## 📊 Key Findings

    Total Vulnerabilities Detected: 135

    Severity Breakdown:

        Critical: 4

        High: 7

        Medium: 3

        Low: 0

        Informational: 121

## 📁 Files

    FirstScan_xw020v.nessus: Raw Nessus export file (machine-readable)

    Nessus_Scan_Report_Summary.pdf: Human-readable summary report in PDF format

## 


# ⚙️ How to Configure Nessus and Run a Scan
## ✅ Step 1: Install Nessus

    Go to the official site: https://www.tenable.com/products/nessus

    Download Nessus for your OS (Windows, Linux, or macOS).

    Run the installer and follow the setup instructions.

    Access the UI at: https://localhost:8834 in your browser.

    Choose:

        Nessus Essentials (free version)

        Enter your email to receive an activation code.

    Finish installation and create an admin account.

## 🛠️ Step 2: Update Plugins

    After registration, Nessus automatically downloads and installs the latest plugins.

    This might take 20-30 minutes.

## 📡 Step 3: Create a New Scan

    From the Nessus dashboard, click "New Scan".

    Choose “Basic Network Scan” or another template based on your goal.

    Fill in scan details:

        Name: e.g., First Internal Scan

        Targets: IP address or hostname (e.g., 192.168.1.10)

        Optional: Add custom policies or credentials if needed.

    Click "Save".

## ▶️ Step 4: Launch the Scan

    Go to the Scans tab.

    Click the Play ▶️ icon next to your saved scan.

    Wait while the scan runs — duration depends on number of targets and scan depth.

## 📈 Step 5: Review and Export Results

    Once completed, click on the scan name to see:

        Vulnerability list

        Severity breakdown

        Affected ports/services

    Use the “Export” button to download results as:

        .nessus (raw XML)

        PDF or HTML (if available)

## 📝 Best Practices

    Scan in a lab environment or with proper authorization.

    Keep Nessus plugins updated for accurate detection.

    Use credentialed scans for deeper insight (with valid SSH/RDP creds).
