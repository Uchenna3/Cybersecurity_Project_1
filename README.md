## ELK Stack Project

### Red Team Resource Group Overview

Diagram below shows full deployment of the RedTeam Resource Group with all the Virtual Artifacts used.


![RedTeam_Resource Group](Images/RedTeam_Resource%20Group.png)

This document contains the following details:

Unit Objectives
Description of the Topology
Access Policies
ELK Configuration
Beats in Use
Machines Being Monitored
How to Use the Ansible Build
Description of the Topology
The main purpose of this network is to expose a load-balanced and monitored instance of DVWA, the D*mn Vulnerable Web Application.

- Craft documentation and interview responses to effectively communicate your achievements. 



Load balancing ensures that the application will be highly available, in addition to restricting in-bound access to the network.

A load balancer intelligently distributes traffic from clients across multiple servers without the clients having to understand how many servers are in use or how they are configured. Because the load balancer sits between the clients and the servers it can enhance the user experience by providing additional security, performance, resilience and simplify scaling your website.
What is the advantage of a jump box?

A jump box is a secure computer that all admins first connect to before launching any administrative task or use as an origination point to connect to other servers or untrusted environments.
Integrating an ELK server allows users to easily monitor the vulnerable VMs for changes to the jumpbox and system network_. -What does Filebeat watch for? Changes to file changes on the machine. -What does Metricbeat record? collect metrics from the operating system and from services running on the server.

The configuration details of each machine may be found below.

Name;	Function;	IP Address;	Operating System;
--------------------------------------------------
Jump Box | Gateway	| Public IP	| Linux
Web-1   | Webserver	| 10.0.0.6 | Linux
Web-2	Webserver	10.0.0.7    |   Linux
Web-3	Webserver	10.0.0.8	Linux
Web-4 (ELK-Server)	Monitoring	10.1.0.4	Linux


### Lab Environment
Personal Azure Environment was used to deply all VM's.

### New VM in Cenrtral Location:

- VM for the ELK server had 8GB of memory for the ELK container to run properly. 
- The New VM was deploed in Central Region.
- Create another vNet in another region and attempt to create the ELK sever in that region.


### Security+ Domains

This unit covers portions of the following domains on the Security+ exam:

<details>
    <summary> Click here to view Security+ Domains that apply to this project. </summary> 
 <br>

- Indicators of compromise
- Types of attacks
- Network components
- Secure network architecture concepts
- Common security issues
- Secure protocols
- Incident response procedures







### Additional Reading and Resources

<details> 
<summary> Click here to view additional reading materials and resources. </summary>
</br>

#### Day 1

- [Elastic: The Elastic Stack](https://www.elastic.co/elastic-stack).
- [Elastic: Filebeat](https://www.elastic.co/beats/filebeat).
- [ELK Docker Documentation](https://elk-docker.readthedocs.io/).
- [Microsoft Azure: Global vNet Peering](https://azure.microsoft.com/en-ca/blog/global-vnet-peering-now-generally-available/)
- [Microsoft Docs: How to open a support ticket](https://docs.microsoft.com/en-us/azure/azure-portal/supportability/how-to-create-azure-support-request)
- [Peachpit.com: Split-Half Search](https://www.peachpit.com/articles/article.aspx?p=420908&seqNum=3)


#### Day 2:

- [Elastic: Filebeat Container Documentation](https://www.elastic.co/beats/filebeat)
- [Phoenixnap.com: Docker Commands Cheat Sheet](https://phoenixnap.com/kb/list-of-docker-commands-cheat-sheet)
- [Boot Camp Resource: Docker and Ansible Cloud Week Cheat Sheet](../12-Cloud-Security/CheatSheet.md)
- [Ansible: Roles Playbook Reuse Roles](https://docs.ansible.com/ansible/latest/user_guide/playbooks_reuse_roles.html)


#### Day 3

- [Elastic: Getting Started with the Elastic Stack](https://www.elastic.co/guide/en/elastic-stack-get-started/current/get-started-elastic-stack.html)

---





---


© 2020 Trilogy Education Services, a 2U, Inc. brand. All Rights Reserved.
