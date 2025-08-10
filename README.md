# JS Extractor Burp Extension

This is a Burp Suite extension written in Python (Jython) that:
- Extracts JavaScript endpoints & parameters
- Downloads external `.js` files
- Avoids duplicates
- Groups by domain
- Adds severity scoring
- Supports clickable table rows to send to Repeater or open in browser
- Auto-constructs missing URLs
- Requests missing JS via CORS with custom headers

## Requirements
- Burp Suite (Community or Pro)
- [Jython Standalone JAR](https://www.jython.org/download)
- Python 2.7 syntax

## Installation
1. Open **Burp Suite → Extender → Extensions → Add**.
2. Extension type: **Python**.
3. Select `js_extractor_jython.py`.
4. Make sure Jython standalone JAR is configured under **Extender → Options**.
