# Cowrie in a nutshell

The Cowrie honeypot can work both as an SSH proxy or as a simulated shell. The emulated shell is pretty convincing 
and could catch an unprepared adversary off guard. Most of the commands work like how you'd expect, and the contents 
of the file system match what would be present on an empty Ubuntu 18.04 installation. 

There are ways to identify this type of Cowrie deployment. For example, it's not possible to execute bash scripts as 
this is a limitation of low and medium interaction honeypots. And when creating a file and then logging back in it
does not exist. It is also possible to identify the default installation as it will mirror a Debian 5 Installation 
and features a user account named Phil. The default file system also references an outdated CPU.

    Intel(R) Core(TM) i9-11900KB CPU @ 3.30GHz

## Cowrie Event Logging

Cowrie uses an extensive logging system that tracks every connection and command handled by the system. It can log 
to a variety of different local formats and log parsing suites. When logging in to the real `ssh` port the logs can
be found in, for example:

    /home/cowrie/honeypot/var/log/cowrie

## Log Aggregation

The amount of data collected by honeypots, especially external deployments can quickly exceed the point where it is 
no longer practical to parse manually. It is often worth deploying Honeypots alongside a logging platform like the 
[ELK stack](blue-siem:docs/elk/README). Other [SIEM platforms]((blue-siem:index)) can provide live monitoring 
capabilities and alerts. This can be particularly beneficial when deploying honeypots with the intent to respond to 
attacks rather than to collect data.

## Resources

* [cowrie/cowrie](https://github.com/cowrie/cowrie)
* [How to send Cowrie output to an ELK stack](https://cowrie.readthedocs.io/en/latest/elk/README.html)
