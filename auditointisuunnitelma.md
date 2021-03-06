# Audit plan #
## Information system X ##
Miespoliisi 2.0
-----

## Change log ##

-----

## Contents ##

-----

# 1 Introduction #

General overview of the system being audited and the related connectivity arrangements.

Roles (owner, users, suppliers - if outsourced)

Target of this evaluation is LDIL's systems related to customer and payment information. Ldil is a national e-tailing company and it also has one physical store with POS-system.

Scope of the evaluation includes systems directly related to customerdata. These systems are web-store, extranet, accounting system, logging system and physical store POS-system.

# 2 Audit target #

Evaluation/Certification: Evaluation

Audit criteria: PCI-DSS

Protection level: N/A 

Timeframe of the audit: N/A

# 3 Applicability #

Parts of organization and processes that are being audited: Systems used by LDIL for managing payment card transactions and other closely related interfaces.

Scopings:

Sampling plan (if applicable)

PCI DSS requirements apply to organizations or entities that store, process or transmit cardholder data or sensitive authentication data. LDIL is an E-commerce company that administers their own E-commerce platform and point of sale systems at their branch store, thus making LDIL's payment system applicable to PCI DSS requirements. 

Storage of sensitive authentication data is forbidden by PCI DSS. On top of PCI DSS requirements, payment card brands can have their own instructions whether storage is permitted prior to authorization. Individual payment card brands requirements are left out the scope of this audit and focus is kept on PCI DSS requirements.

3.1 Scoping

Purpose of scoping is to determine which components of LDIL's business environment are part of cardholder data environment. Cardholder data environment comprises of LDIL's payment system components and all other connected systems.

Determining the scale of cardholder data environment is done by reviewing LDIL's provided documentation of the current business environment and security measures. Once the cardholder data environment and cardholder data flow in the payment system is identified and documented, the determined PCI DSS scope is reviewed by the LDIL before beginning the assesment (at least in real life case). 

LDIL cardholder data environment (according to LDIL documentation fig. 1, page 8):

* Magento server (E-commerce platform, payment system component)
* All other hosts in DMZ network segment (located at the same segment as Magento)
* POS Cyclos (payment system component)
* All other hosts in Store brach network segment (located at the same segment as POS)
* Paloalto and PFsense firewalls (essential network infrastructure)

Magento and Cyclos should be studied at application level to have greater knowledge about their functionality. If applications
use for example external database server it has impact on the scope of cardholder data environment.

# 4 Auditors #

Head auditor(s):

Supplementary auditors:

(Pääarvioijan vastuut, jos soveltuu)

# 5 Audit activities and schedule #

## 5.1 Schedule and premilinary work estimate #

Alustavan yhdessä XXX kanssa sovitun aikataulun mukaan...

Premilinary work estimate:

 * Reviewing the material, planning and technical implementation:
 * Review of administration and monitoring systems:
 * Review of the ISMS including administration procedures and practices:
 * Review of business continuity:
 * Review of reporting procedures:
 * Reporting:
 * Total:

(Mahdollista taulukkoa eri osa-alueista, esim. salausratkaisut, tekninen arviointi, passiivinen rajapinta-analyysi...: Henkilöt/Asiakkaan edustaja, vastuullinen arvioija, Arviointi/tarkastus pvm.)

## 5.2 Administrative and technical reviews of named technologies

### 5.2.1 Network and systems security

 1. Technical review
    * Review of firewall rules and configurations against the documentation
    * Verification of documented zoning using scans and traffic capture
    
 2. Administrative review
    * Change management of router and firewall rule and configuration changes
    * Secure and documented settings, including e.g. ports and protocols
    * Network diagrams
    * Administrative roles
    * Regular configuration review

### 5.2.2 Configuration defaults

 1. Technical review
    * Verification that default passwords and other configuration parameters have been changed
    * Hardening of systems
    * Separation of server roles
    * Disabling unnecessary protocols, services etc.
    * Secure administration channels

 2. Administrative review
    * Configuration management

### 5.2.3 Data protection

 1. Technical review
    * Verify that no undocumented cardholder data persists in the systems
    * Verify the documented data is masked
    * Verify the security of encryption and encryption keys

 2. Administrative review
    * Documentation of stored cardholder data

### 5.2.4 Security of data transmissions

 1. Technical review
    * By reviewing configuration and traffic verify that required data is transferred properly encrypted

 2. Administrative review
    * Encryption strength
    * Encryption policies

### 5.2.5 Malware protection

 1. Technical review
    * Antivirus programs are installed in necessary systems
    * Antivirus programs are regularly updated
    * Antivirus programs successfully detect test malware

 2. Administrative review
    * Awareness of current virus and malware threath

### 5.2.6 Secure systems and applications

 1. Technical review
    * Software updates are regularly applied
    * Software is scanned for vulnerabilities
    * Outer edge of network is scanned for vulnerabilities and undocumented services

 2. Administrative review
    * Update procedures for software
    * Identification of required updates
    * Regular software scans
    * Change control

### 5.2.7 Access restrictions to data

 1. Technical review
    * Review that unnecessary access to cardholder data is prevented

 2. Administrative review
    * Needed access rights are documented

### 5.2.8 Access restrictions to systems

 1. Technical review
    * Verify user identification from configurations
    * Verify limitations of user access
    * Verify documented logging, connection and password policies

 2. Administrative review
    * User ID policy
    * Password policy
    * Training of personnel for secure settings

### 5.2.9 Monitoring and testing

 1. Technical review
    * Verification of generated audit logs
    * Separation of duties
    * Log preservation

 2. Administrative review
    * Audit log policy
    * Documented separation of duties

### 5.2.10 Testing security systems and processes

 1. Technical review
    * Audit IDS/IPS and HIDS exists and is correctly configured

 2. Administrative review
    * Policy for regular testing, scanning and penetration testing
    * Existing scan reports

### 5.2.11 Information security policy

 1. Technical review

 2. Administrative review
    * Security policy
    * Risk assessment policy
    * Usage policies
    * Inventories and ownerships
    * Information security management
    * Training of personnel
    * Personnel screening
    * Incident response plan

# 6 Reporting #

Meeting minutes

Report


DISTRIBUTION
