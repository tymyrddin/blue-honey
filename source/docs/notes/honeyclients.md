# Honeyclients

For most honeypots to work, you have to wait for the attacker to attack the honeypot from a remote location. This ignores that most attacks are client-side. A phishing e-mail arrives in an inbox, the user clicks and allows the remote malware to activate on the device and allows it to callback over TCP port 80, which is allowed by most firewalls.

Meanwhile, drive-by downloads overtook file attachment phishing as the major means of initial access. Enter client-side honeypots (honeyclients), to track and analyse these types of attacks.

A honeyclient mimics, either manually or automatically, the normal series of steps a regular user would make when visiting websites. It can be fully patched or be left vulnerable. The idea is to identify malware hosts, and possibly even gather attribution information.

![Web honeypots](../../_static/images/web.png)

HoneyMonkey (dead since 2010) was a web browser based (IE) high interaction client honeypot built by Microsoft in 2005. It detected attacks on clients by monitoring files, registry, and processes.

[Thug](https://github.com/buffer/thug) is a Python low-interaction honeyclient aimed at mimicing the behaviour of a web browser in order to detect and emulate malicious contents. It is actively being developed. Many more such honeyclients exist.

