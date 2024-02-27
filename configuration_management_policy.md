# Configuration Management Policy

Janus Healthcare Partners standardizes and automates configuration management through the use of Ansible scripts as well as documentation of all changes to production systems and networks. Ansible automatically configures all Janus Healthcare Partners systems according to established and tested policies, and is used as part of our Disaster Recovery plan and process.

## Applicable Standards from the HITRUST Common Security Framework

* 12 - Configuration Management

## Applicable Standards from the HIPAA Security Rule

* 164.310(a)(2)(iii) Access Control & Validation Procedures

## Configuration Management

1. Ansible is used to standardize and automate configuration management.
2. No systems are deployed into Janus Healthcare Partners environments without approval of the Janus Healthcare Partners CTO.  Only authorized administrators can implement such upgrades to software, application, and program libraries.  All upgrades are based on business requirements and applicable security implications.
4. All changes to production systems, network devices, and firewalls are approved by the Janus Healthcare Partners CTO before they are implemented. Additionally, all changes are tested before they are implemented in production.
5. An up-to-date inventory of systems is maintained. All systems are categorized as production and utility to differentiate based on criticality.
6. Clocks are synchronized across all systems using NTP. Modifying time data on systems is restricted.
7. All front end functionality (developer dashboards and portals) is separated from backend (database and app servers) systems by being deployed on separate servers.
8. All software and systems are tested using end-to-end tests.
9. All committed code is reviewed using pull requests GitHub to assure software code quality and proactively detect potential security issues in development.
10. Janus Healthcare Partners utilizes development and staging environments that mirror production to assure proper function.
11. All formal change requests require unique ID and authentication.
