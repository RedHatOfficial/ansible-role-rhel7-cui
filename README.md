Unclassified Information in Non-federal Information Systems and Organizations (NIST 800-171)
=========

Ansible Role for Unclassified Information in Non-federal Information Systems and Organizations (NIST 800-171)  
  
Profile Description:  
From NIST 800-171, Section 2.2:  
Security requirements for protecting the confidentiality of CUI in non-federal  
information systems and organizations have a well-defined structure that  
consists of:  
(i) a basic security requirements section;  
(ii) a derived security requirements section.  
The basic security requirements are obtained from FIPS Publication 200, which  
provides the high-level and fundamental security requirements for federal  
information and information systems. The derived security requirements, which  
supplement the basic security requirements, are taken from the security controls  
in NIST Special Publication 800-53.  
This profile configures Red Hat Enterprise Linux 7 to the NIST Special  
Publication 800-53 controls identified for securing Controlled Unclassified  
Information (CUI).

The tasks that are used in this role are generated using OpenSCAP.
See the OpenSCAP project for more details on Ansible playbook generation at [https://github.com/OpenSCAP/openscap](https://github.com/OpenSCAP/openscap)

To submit a fix or enhancement for an Ansible task that is failing or missing in this role,
see the ComplianceAsCode project at [https://github.com/ComplianceAsCode/content](https://github.com/ComplianceAsCode/content)

Requirements
------------

- Ansible version 2.9 or higher

Role Variables
--------------

To customize the role to your liking, check out the [list of variables](defaults/main.yml).

Dependencies
------------

N/A

Example Role Usage
----------------

Run `ansible-galaxy install RedHatOfficial.rhel7_cui` to
download and install the role. Then, you can use the following playbook snippet to run the Ansible role:

    - hosts: all
      roles:
         - { role: RedHatOfficial.rhel7_cui }

Next, check the playbook using (on the localhost) the following example:

    ansible-playbook -i "localhost," -c local --check playbook.yml

To deploy it, use (this may change configuration of your local machine!):

    ansible-playbook -i "localhost," -c local playbook.yml

License
-------

BSD-3-Clause

Author Information
------------------

This Ansible remediation role has been generated from the body of security
policies developed by the ComplianceAsCode project. Please see
[https://github.com/complianceascode/content/blob/master/Contributors.md](https://github.com/complianceascode/content/blob/master/Contributors.md)
for an updated list of authors and contributors.
