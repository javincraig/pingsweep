# pingsweep
Multi Thread Ping Sweep forked from Rubysash and modified to fit my needs

# Description
pingsweep.py - is multi threaded (scans /24 in about 10s)

This sends 3 pings and if there is a response it adds it to a list.
Once the sweep is complete, it prints it out (currently)

It uses the ipaddress module so you can specify just about any CIDR you want.
From the CIDR specified it will:

* build a list of ip addresses to scan
* loop over that list, checking for specified timeout, unreachable or "Reply/bytes"
* sort final replies and print them
* give timed result and hosts found count
