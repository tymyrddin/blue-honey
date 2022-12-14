# Yalih

[YALIH](https://github.com/Masood-M/yalih) (Yet Another Low Interaction Honeyclient) is a low Interaction Client 
honeypot designed to detect malicious websites through signature, anomaly and pattern matching techniques. YALIH 
has the following capabilities:

* Suspecious URL collection from malicious website databases (three databases)
* URL collection through Bing API
* Suspecious URL collection from your inbox and SPAM folder through pop3 and IMAP protocol
* Javascript extraction, de-obfuscation and de-minification of scripts embedded within a website
* Referrer Emulation and redirection handling
* Cookies and session handling
* Browser and browser agent and OS emulation
* Proxy capabilities to detect Geo-location and/or IP cloacking attacks
* Signature detection using ClamAV antivirus database
* Anomaly and pattern matching detection through Yara (http://plusvic.github.io/yara/)
* Automated Yara signature generation