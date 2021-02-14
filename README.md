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

|   Name       |	Function    | IP Address |	Operating System|
| ------------ |----------------| -----------|------------------|
|   Jump Box   | Gateway	| Public IP	    | Linux
|   Web-1      | Webserver	| 10.0.0.6      | Linux
|   Web-2	   | Webserver	| 10.0.0.7      | Linux
|   Web-3	   | Webserver	| 10.0.0.8	    | Linux
| Web-4 (ELK-Server) |	Monitoring	| 10.1.0.4 |	Linux


### Lab Environment
Personal Azure Environment was used to deply all VM's.

### New VM in Cenrtral Location:

- VM for the ELK server had 8GB of memory for the ELK container to run properly. 
- The New VM was deploed in Central Region.
- Create another vNet in another region and attempt to create the ELK sever in that region.

### Access Policies
The machines on the internal network are not exposed to the public Internet.

Only the jump box provisioner machine can accept connections from the Internet. Access to this machine is only allowed from the following IP addresses:

5061 Kibana Port
Machines within the network can only be accessed by jump box provisioner.

Which machine did you allow to access your ELK VM?

My IP Address: 99.122.6.55
A summary of the access policies in place can be found in the table below.

|   Name     | Public Access| IP Addresses|
| ---------- |--------------|-------------|
| Jumpbox    | Yes          | 
| Web-1      | No           |   10.0.0.6  |
| Web-2      | No           |   10.0.0.7  |
| Web-3      | No           |   10.0.0.8  |
| Web-4 ELK  | No           |   10.1.0.4  |

Ansible was used to automate configuration of the ELK machine. No configuration was performed manually, which is advantageous because... What is the main advantage of automating configuration with Ansible?

Free: Ansible is an open-source tool.
Very simple to set up and use: No special coding skills are necessary to use Ansible’s playbooks (more on playbooks later).
Powerful: Ansible lets you model even highly complex IT workflows.
Flexible: You can orchestrate the entire application environment no matter where it’s deployed. You can also customize it based on your needs.
Agentless: You don’t need to install any other software or firewall ports on the client systems you want to automate. You also don’t have to set up a separate management structure.
Efficient: Because you don’t need to install any extra software, there’s more room for application resources on your server.
The playbook implements the following tasks:

Install docker.io
Install pip3
Install Docker python module
Increase virtual memory
Download and launch a docker
The following screenshot displays the result of running docker ps after successfully configuring the ELK instance.


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
