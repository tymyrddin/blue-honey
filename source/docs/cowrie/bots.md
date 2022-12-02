# Bot intrusions

## Typical bot activity

The majority of attacks against typical SSH deployments are automated in some way. As a result, most of the 
post-exploitation activity that takes place after a bot gains initial access to the honeypot will follow a broad 
pattern. Most bots will perform a combination of the following:

* Perform some reconnaissance using the `uname` or `nproc` commands or by reading the contents of files like 
`/etc/issue` and `/proc/cpuinfo`. It is possible to change the contents of all these files so the honeypot can pretend 
to be a server or even an IoT toaster.
* Install malicious software by piping a remote shell script into bash. Often this is done using `wget` or `curl`. 
On occasion `FTP` is used. Cowrie will download each unique occurrence of a file but prevent the scripts from 
being executed. Most of the scripts tend to reference cryptocurrency mining in some way.
* A more limited number of bots will do some anti-forensics tasks by deleting various logs and disabling bash history. 
This does not affect Cowrie since all the actions are logged externally.

Bots are not limited to these actions in any way and there is still some variation in the methods and goals of bots. 

## Bot Identification

It is possible to use the data recorded by Cowrie to identify individual bots. The factors that can identify traffic 
from individual botnets are not always the same. However, some artifacts tend to be consistent across bots including 
the IP addresses requested by bots and the specific order of commands. Identifiable messages may also be present 
in scripts or commands though this is uncommon. Some bots may also use highly identifiable public SSH keys to 
maintain persistence.

It is also possible to identify bots from the scripts that are downloaded by the honeypot, using the same methods 
that would be used to identify other malware samples. 