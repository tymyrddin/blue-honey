# Attacks against SSH

By default, Cowrie will only expose SSH. This means adversaries will only be able to compromise the honeypot by 
attacking the SSH service. The attack surface presented by a typical SSH installation is limited so most attacks 
against the service will take the form of brute-force attacks. Defending against these attacks is relatively simple 
in most cases as they can be defeated by only allowing public-key authentication or by using strong passwords. 
These attacks should not be completely ignored, as there are simply so many of them that you are pretty much 
guaranteed to be attacked at some point.

Arguably the most common tool for brute-forcing SSH is Hydra, and commonly fail2ban is used to mitigate SSH 
brute-force attacks.


