## ELK Stack Project

### Unit Description

Diagram below shows full deployment of the RedTeam Resource Group with all the Virtual Artifacts used.

![RedTeam_Resource Group.png]

### Unit Objectives

<details>
    <summary>Click here to view the daily unit objectives.</summary>

  <br>

Throughout this week, you will apply skills and knowledge gained over the past twelve weeks to complete the following: 

- Deploy containers using Ansible and Docker.

- Deploy Filebeat using Ansible.

- Deploy the ELK stack on a server.

- Diagram networks and creating a README.

- Craft documentation and interview responses to effectively communicate your achievements. 

</details>


### Lab Environment

For the majority of demonstrations and activities, the class will use Microsoft Azure cloud services and the Azure cloud portal.

- You will **not** be using any of the Azure lab environments. Instead, you will be using personal Azure accounts.

### What to Be Aware Of:

- The sample logs used in this unit are specific to the time in which they are viewed. As such, answers will vary from the answers provided in the solutions.

- The VM for the ELK server **must** have at least 4GiB of memory for the ELK container to run properly. Azure has VM options that have `3.5 GiB` of memory, but **do not use them**. They will not properly run the ELK container because they do not have enough memory.

- Azure may run out of available VMs for you to create a particular region. If this happens, you will need to do one of two things:

  - Open a support ticket with Azure support using [these instructions](https://docs.microsoft.com/en-us/azure/azure-portal/supportability/how-to-create-azure-support-request). Azure support is generally very quick to resolve issues.

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


</details> 

<br>

For more information about these Security+ domains, refer to the following resource: [Security+ Exam Objectives](https://www.comptia.jp/pdf/Security%2B%20SY0-501%20Exam%20Objectives.pdf)


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


</details>



### Unit 13 : Homework

This unit's homework assignment can be viewed here:

- [Unit 13 Homework File](../../2-Homework/13-Github-Fundamentals/Unsolved/README.md)

### Looking Forward 

The next unit will mark the start of the Offensive Security module. In the Web Development unit, we'll examine the infrastructure and deployment of web applications to inform how we can explore and exploit vulnerabilities within those applications.  



---


© 2020 Trilogy Education Services, a 2U, Inc. brand. All Rights Reserved.
