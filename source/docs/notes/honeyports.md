# Honeyports

Consider [honeyports](https://github.com/gchetrick/honeyports), an effective defence for air gapped/high security networks:

* They give you visibility.
* Current IDS IPS technologies fail at detecting attackers communicating with open ports over normal protocols (SMB, SSH, HTTP, and HTTPS). Some Next-Gen firewalls already have some of the deception capabilities.
* Most IPS/IDS technologies are still blind at detecting 0-day attacks. 
* If anyone interacts with a honeyport, it can trigger an alert and/or create a dynamic blacklist entry.
* You can run them from the command line, and you can run them as Python, PowerShell, and Ruby scripts.

## How it works

Create a non-legitimate listening port on an external facing legitimate non-important server that are favorite for remote attacks, like telnet or ssh. The services need not be installed. Listen on that port using tools like honeyports. 

Most pentesters, redteamers and adversaries start with reconnaissance. When an attacker runs a recon scan against this server, sees this open port and tries to communicate, automatically block that IP at your perimeter so that all further actions are blocked.

Take that a step further and check out [portspoof](https://drk1wi.github.io/portspoof/). A port scan will take ages and becomes utterly meaningless with every port responding that it is up and running some service. Scanning tools will try to enumerate those services by running additional checks, over ***`65536`*** ports.

## Resources

* [Active Defense, Offensive Countermeasures, and Cyber Deception](https://www.blackhillsinfosec.com/wp-content/uploads/2020/04/Training_ActiveDefence_CyberDeception_April2020.pdf), John Strand, Bryce Galbraith and Paul Asadoorian, 2020

