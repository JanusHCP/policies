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

## Change Management
Janus HCP seeks to minimize risks associated with changes or configurations to applicaionts, operating systems, patch levels, and other IT infastructure.  Changes are defined as any modification, addition, or removal of anything from and applicaionts, an operating systems, patch levels, and other IT infastructure.  All changes must be implementd given the apoval framework outlined in the configuration management policy including aproval & review of all changes by the CTO and implemenation of all changes by privlidged IT professionals only.  Changes are classified as:

1. Standard - The type of change performed on a routine basis and follows an established framework
2. Major - The type of change with a large impact on a specific system, requries a lot of dependencies, or requries changes significant accomodations.
3. Minor - The type of change with a very minimal impact on the applicable system
4. Emergency - The type of change in response to a high impact problem that requries an urgent fix.

All changes regardless of classification are reviewed using GitHup pull requests and are aproved, reviewed, and logged using the Configuration Management Form.
