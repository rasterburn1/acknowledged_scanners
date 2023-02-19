# Acknowledged Scanners - FAQ

## Metadata

Version 1.0 -- September 23, 2021

## What is this? 

The acknowledged scanner repository tracks the ip addresses and other indicia of scanners which, _we believe_ are non-hostile.  Acknowledged scanners interact with the larger world in a number of ways, including:
- Providing public information on what they're scanning.
- Providing a service based on their scan data, such as a search engine, threat intelligence, or another security or networking quality product.
- Engaging with the research community by providing data in published papers, reports, etc. 
- Providing an opt-out.

## Are these scans attacks/are these scans not attacks? 

We don't know.  We call these scanners "acknowledged" as opposed to "non-hostile" because these scanners who have made an effort to make themselves known.  Outside of that, there is a spectrum of behavior.

## Why does this matter?

Acknowledged scanners behave differently than run-of-the-mill hostile scanners.  At a glance, they scan a wider variety of ports, and their behavior is less predictable on a daily basis (we hypothesize that this is because most acknowledged scanners are staggering a large number of different portscans, while the run-of-the-mill scanners are focusing on ports they have specific exploits for).  For researchers, this results in two different models of behavior, while for operators its a potential source of false positives. 

## What does this repository contain?
At this time, a list of approximately 40 known scanners and their observed IP addresses.  
- The ''orgs.csv'' file contains a list of the organizations
- A utility, 'asutil.py' which will create lists of acknowledged scanner ips
- A list of IP addresses, broken down by scanners

This is a first release
