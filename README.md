# Acknowledged Scanners - FAQ

## Metadata

Version 1.0 -- November 12, 2024

## What is this? 

This repository tracks the ip addresses of not only scanners which, are assumed to be non-hostile, but also those used by the Bad Actors.  Acknowledged scanners interact with the larger world in a number of ways, including:
- Providing public information on what they're scanning.
- Providing a service based on their scan data, such as a search engine, threat intelligence, or another security or networking quality product.
- Engaging with the research community by providing data in published papers, reports, etc. 
- Providing an opt-out.

The Bad Actors interact with the larger world in a number of other ways, including:
- Using exploits to gain access to services.
- Attempting to log in to available services.
- Testing/Attempting to/Successfully making unauthorised usage of available/open/unsecured services (often made known to the public by Acknowledged scanners).
- etc. etc.

## Are these scans attacks/are these scans not attacks? 

We don't know.  We call these scanners "acknowledged" as opposed to "non-hostile" because these scanners who have made an effort to make themselves known.  Outside of that, there is a spectrum of behavior.

## Why does this matter?

Acknowledged scanners behave differently than run-of-the-mill hostile scanners.  At a glance, they scan a wider variety of ports, and their behavior is less predictable on a daily basis (we hypothesize that this is because most acknowledged scanners are staggering a large number of different portscans, while the run-of-the-mill scanners are focusing on ports they have specific exploits for).  For researchers, this results in two different models of behavior, while for operators its a potential source of false positives. 

## What does this repository contain?
At this time, a list of 40+ known scanners and their observed IP addresses.  
- The directory 'acknowledged scanners' contains an updated version of [Michael Collins' Acknowledged Scanners Repository](https://gitlab.com/mcollins_at_isi/acknowledged_scanners)
    - The names have been updated and the files have been formatted for use by ipset directly
- Seperate lists of IP addresses, broken down by scanners
- Each scanners IP (IPv4 and IPv6 where applicable) address list individually formatted for use (as a direct "restore" file) with ipset
- A complete (IPv4 and IPv6) list formatted for use (as a direct "restore" file) with ipset

This is a first release
