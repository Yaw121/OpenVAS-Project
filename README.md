### Azure Vulnerability Management Lab: Assessing and Remediating Security Risks with OpenVAS

![image](https://github.com/user-attachments/assets/4fcbf238-c7f6-43f9-a5b7-71c42bcb741a)

### Introduction:
In this lab, I will go through the process of setting up a vulnerability management environment in Azure. I look to learn how to configure and utilize OpenVAS, a vulnerability scanner, to identify and assess security vulnerabilities in a Windows virtual machine (VM). Additionally, I will perform uncredentialed scans, and credentialed scans, apply remediations, and verify the effectiveness of the remediation measures.

STEPS

<details>
  <summary><b>Task 1: Prepare the Vulnerability Management</b></summary>
  
 - Access the Azure Portal and navigate to the Marketplace.
 - Search for "OpenVAS secured and supported by HOSSTED" and select it.
 - Choose a pre-set configuration and create the VM with specified settings.
 - ![Screenshot 2024-12-08 004501](https://github.com/user-attachments/assets/e619016e-46d4-4926-9a3e-09c6f789796d)
 - Virtual Machine Settings
   
| Setting      |   Value      |
|----------------|----------------|
| Resource Group | Vulnerability-Management |
| VM Name: | OpenVAS (Take note of the region and Vnet–consider East US ) |
| Region: | East US (make sure to note the region and Vnet) |
| Authentication: | Password (Provide Username/Password) |



</details>
