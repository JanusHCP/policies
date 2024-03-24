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

## Segregation of Duties
Developers have the privileged to deploy code only with the explicit approval of the CTO.  All developer code is peer reviewed using GitHub pull requests as explained in part 9 of Configuration Management.  Peer approved code can be deployed by developers to the Janus staging environment only.  Code can only be deployed to the Janus production environment with explicit written approval of the CTO via the change management form.  Only approved and trained developers have access to the Janus platform code and have the privilege to push code to staging or production.

## Change Management
Janus HCP seeks to minimize risks associated with changes or configurations to applications, operating systems, patch levels, and other IT infrastructure.  Changes are defined as any modification, addition, or removal of anything from and applications, an operating systems, patch levels, and other IT infrastructure.  All changes must be implemented given the approval framework outlined in the configuration management policy including approval & review of all changes by the CTO and implementation of all changes by privileged IT professionals only.  Changes are classified as:

1. Standard - The type of change performed on a routine basis and follows an established framework
2. Major - The type of change with a large impact on a specific system, requires a lot of dependencies, or requires changes significant accommodations.
3. Minor - The type of change with a very minimal impact on the applicable system
4. Emergency - The type of change in response to a high impact problem that requires an urgent fix.

All changes regardless of classification are reviewed using GitHub pull requests and are approved, reviewed, and logged using the Configuration Management Form.  All changes are deployed to the Janus staging environment for review by CTO before being deployed to production.

## Patch Management
The Janus Patch Management Policy dictates how patches are deployed to physical IT infrastructure (employee workstations) and the Janus HCP servers hosted on AWS.  Note, Janus Healthcare Partners does not use any on site servers, networking devices, or mobile devices.  

1. Janus HCP uses a remote scripting software to run scripts pushing security related patches remotely and instantly to employee workstations.  This is not done through GPO but through scripting software triggered via out inventory management tool, Datto.
2. Janus HCP uses the AWS Patch Manager to push updates, including security related patches, to the Janus server platform.
3. All patches are classified, evaluated, and prioritized by:

   a. Standard - The type of patch performed on a routine basis and follows an established framework.  Standard patches are of the lowest priority and are pushed on a pre- 
                  determined schedule.

   b. Major - The type of patch with a large impact on a specific system, requires a lot of dependencies, or requires changes significant accommodations.  Major patches   
               are prioritized ahead of Standard and Minor patches.  Major patches are pushed out on a schedule to accommodate necessary review of dependencies or impacted   
               systems.

   c. Minor - The type of patch with a very minimal impact on the applicable system.  Minor patches are prioritized ahead of Standard but behind Major patches.

   d. Emergency - The type of patch in response to a high impact problem that requires an urgent fix.  Emergency patches are prioritized overall other fixes.

5. Workstations are configured to force the installation of all updates pushed by windows or other installed approved software's.  User do not have admin access and cannot override or disable this configuration.
