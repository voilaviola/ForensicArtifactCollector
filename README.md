# ForensicArtifactCollector
Bulk &amp; Remote Forensic Artifact Collector using DumpIt.exe and other tools

Generate a new file computer_profiles.txt in Sessions\, to help determine Win10 volatility profile
Artifact Collector is a stand-alone application aimed at facilitating data acquisition for incident response and threat hunting on Windows. 

# Usage Instruction
There are 2 ways to use this application: 
>	1. Place the ArtifactCollector.exe on an external disk, connect this disk to target PC, and double click to launch the exe (as shown in the video)
>	2. Place the ArtifactCollector.exe on a shared network drive, access the shared drive from the traget PC, and double click to launch the exe
Administrator priviledge is needed in both ways. And path to the .exe cannot contain space " " or slashes "/" "\\"
The application creates in its directory a "Sessions" folder, in which "MemoryImages" contains raw memory image of target PC, and "COMPUTERNAME_TIMESTAMP" contains other artifacts. 
All temporary files created by this application will be deleted from target PC when the collection finishes.

# Artifacts Collected 
Drivers : imports, exports, digital signatures, MD5
Event logs
Network : ARP, DNS, routing table, port enumeration
System & OS : Machine & OS information, Registry hive, User accounts, Prefetch
Services : MD5, Digital signature
Tasks : MD5, Digital signature
Browser : Cookies, from history, file download history, url history

