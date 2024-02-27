# Introduction

Janus Healthcare Partners ("Janus Healthcare Partners") is committed to ensuring the confidentiality, privacy, integrity, and availability of all electronic protected health information (ePHI) it receives, maintains, processes and/or transmits on behalf of its customers. As providers of compliant, hosted infrastructure used by health technology vendors, developers, designers, agencies, custom development shops, and enterprises, Janus Healthcare Partners strives to maintain compliance, proactively address information security, mitigate risk for its Customers, and assure known breaches are completely and effectively communicated in a timely manner. The following documents address core policies used by Janus Healthcare Partners to maintain compliance and assure the proper protections of infrastructure used to store, process, and transmit ePHI for Janus Healthcare Partners Customers.

## Compliance Inheritance

Janus Healthcare Partners provides compliant software for its Customers.

Janus Healthcare Partners signs business associate agreements (BAAs) with its Customers. These BAAs outline Janus Healthcare Partners obligations and Customer obligations, as well as liability in the case of a breach. In providing infrastructure and managing security configurations that are a part of the technology requirements that exist in HIPAA and HITRUST, as well as future compliance frameworks, Janus Healthcare Partners manages various aspects of compliance for Customers. The aspects of compliance that Janus Healthcare Partners manages for Customers are inherited by Customers, and Janus Healthcare Partners assumes the risk associated with those aspects of compliance. In doing so, Janus Healthcare Partners helps Customers achieve and maintain compliance, as well as mitigates Customers risk.

Certain aspects of compliance cannot be inherited. Because of this, Janus Healthcare Partners Customers, in order to achieve full compliance or HITRUST Certification, must implement certain organizational policies. These policies and aspects of compliance fall outside of the services and obligations of Janus Healthcare Partners.

Below are mappings of HIPAA Rules to Janus Healthcare Partners controls and a mapping of what Rules are inherited by Customers, both Add-on Customers and SaaS Customers.

## Janus Healthcare Partners Organizational Concepts

The physical infrastructure environment is hosted at Google Cloud Platform (GCP). The network components and supporting network infrastructure is contained within GCP infrastructure and managed by GCP. Janus Healthcare Partners does not have physical access into the network components. The Janus Healthcare Partners environment consists of firewalls, ElasticSearch, Postgres database servers, Google Cloud Spanner, CockroachDB database servers, Google Cloud Datastore, Google Cloud PubSub, Logstash logging servers, Prometheus logging servers, Linux Ubuntu servers, and developer tool servers running on Linux Ubuntu.

Within the Janus Healthcare Partners Platform all data transmission is encrypted and all hard drives are encrypted so data at rest is also encrypted; this applies to all servers - databases, APIs, log servers, etc. Janus Healthcare Partners assumes all data *may* contain ePHI, even though our Risk Assessment does not indicate this is the case, and provides appropriate protections based on that assumption.

## Version Control

Policies were last reviewed and updated December 21th, 2023.

Policies were written by Michael Wasser, CTO.

Policies were approved by Richard Clarke, COO.
