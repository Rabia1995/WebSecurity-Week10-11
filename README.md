# Project 9 - Honeypot

Time spent: **8** hours spent in total

> Objective: Setup a honeypot and intercept and attempted attacks in the wild.

## Honeypots Deployed

### Dionaea Sensor
Dionaea is "the Nepenthes successor"a malware capturing honeypot. Dionaea aims to trap malware exploiting vulnerabilities exposed by services offered over a network, and ultimately obtain a copy of the malware.

### Snort Sensor
Snort is an "open source intrusion prevention system capable of real-time traffic analysis and packet logging."

### Amun Sensor
Amun is a "python-based low-interaction honeypot, following the concepts of Nepenthes but extending it with more sophisticated emulation and easier maintenance."

## Problem Encountered
I had trouble with Milestone 1 about creating the MHN Admin VM. The instructions were a little confusing so it took me some time to figure it out.

I also had trouble with downloading the session.json file, so I did it by dumping the data using

```# Dump all the records from the session collection```

```mongoexport --db mnemosyne --collection session > session.json```

```# Dump the source_ip and destination_ip fields from the session collection as JSON```

```mongoexport --db mnemosyne --collection session --fields=source_ip,destination_ip``` 


## Summary of Data

<img src="https://github.com/Rabia1995/WebSecurity-Week10-11/blob/master/Screenshot%201.png">

## 

<img src="https://github.com/Rabia1995/WebSecurity-Week10-11/blob/master/Screenshot%202.png">
