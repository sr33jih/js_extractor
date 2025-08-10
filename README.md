JavaScript Endpoint Extractor for Burp Suite
Description
This is a Burp Suite Jython extension that automatically detects and extracts endpoints and parameters from JavaScript files while you browse or scan a target.
It can also:

Download and store external .js files linked in HTML.

Avoid duplicates to save processing time.

Group results by domain.

Assign severity scores based on findings.

Provide clickable results so you can send them to Repeater or open them in a browser.

Features
🔍 Extract endpoints & parameters from inline and external JS.

🌐 Auto-download external .js files from HTML.

📁 No duplicates — each file is stored only once.

📊 Group by domain for better organization.

⚠️ Severity scoring based on matched patterns.

🔄 Auto-fetch missing JS from CORS/remote hosts with custom headers.

🖱️ Right-click actions — send entries directly to Burp Repeater or browser.

🔗 Auto-URL construction for partial paths.

Installation (Burp Suite)
Download the js_extractor_jython.py file from this repository.

Download and install Jython Standalone:

Get jython-standalone-2.7.3.jar from https://www.jython.org/download.html

Open Burp Suite → Extender → Options → Python Environment.

Point Burp to your jython-standalone-2.7.3.jar.

Go to Extender → Extensions → Add.

Set:

Extension type: Python

Extension file: select js_extractor_jython.py

Click Next — the extension should load without errors.

Requirements
Burp Suite (Community or Professional)

Jython Standalone 2.7.x

Internet access (for downloading external JS)

Python 2.7 syntax compatibility (Jython environment)

Usage Instructions
Load the extension in Burp as described in the installation steps.

Start proxying traffic or use Burp's crawler/scanner to load target pages.

The extension will automatically:

Identify .js files (inline and external).

Download and store external .js files.

Extract endpoints and parameters.

View results in the extension’s tab in Burp:

Results are grouped by domain.

Severity scores are displayed.

Right-click any row to:

Send to Repeater.

Open in browser.

Export results to a file for later analysis.
