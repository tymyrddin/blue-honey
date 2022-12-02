# SSH tunnelling

Some bots will not perform any actions directly against honeypot and instead will leverage a compromised SSH 
deployment itself. This is done with the use of SSH tunnels. SSH tunnels forward network traffic between nodes 
via an encrypted tunnel. SSH tunnels can add a layer of secrecy when attacking other targets as third parties are 
unable to see the contents of packets that are forwarded through the tunnel. Forwarding via SSH tunnels also 
allows an adversary to hide their true public IP in much the same way a VPN would.

The IP obfuscation can then be used to facilitate schemes that require the use of multiple different public IP 
addresses like SEO boosting and spamming. SSH tunnelling may also be used to by-parse IP-based rate limiting tools 
like Fail2Ban as an adversary is able to transfer to a different IP once they have been blocked.

## SSH tunnelling data in Cowrie

By default, Cowrie will record all SSH tunnelling requests received by the honeypot, but will not forward them on to 
their destination. This data is of particular importance as it allows for the monitoring and discovery of web attacks 
that may not have been found by another honeypot. 