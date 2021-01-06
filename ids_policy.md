# IDS Policy

In order to preserve the integrity of data that BloomAPI stores, processes, or transmits for Customers, BloomAPI implements strong intrusion detection tools and policies to proactively track and retroactively investigate unauthorized access. 

## Applicable Standards from the HITRUST Common Security Framework

*  09.ab - Monitoring System Use
*  06.e - Prevention of Misuse of Information
*  10.h - Control of Operational Software

## Applicable Standards from the HIPAA Security Rule

* 164.312(b) - Audit Controls

## Intrusion Detection Policy

* BloomAPI firewalls monitor all incoming traffic to detect potential denial of service attacks. Suspected attack sources are blocked automatically. Additionally, our hosting provider actively monitors its network to detect denial of services attacks.
* All new firewall rules and configuration changes are tested before being pushed into production. All firewall and router rules are reviewed bi-annually by the engineering team.
* BloomAPI utilizes redundant firewall on network perimeters.
* Static IP addresses are used for BloomAPI servers.
