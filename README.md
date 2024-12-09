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

![image](https://github.com/user-attachments/assets/2f5bd5cb-5648-49fc-9da6-edded6931adc)

- On the Disk Tab, Networking, Management, and Advanced we will let them remain as their default Settings.

- For the Monitoring tab, we will disable boot diagnostics as it will not be needed in the lab. You can learn more about boot diagnostics 
<a href=https://learn.microsoft.com/en-us/azure/virtual-machines/boot-diagnostics>here</a>

![image](https://github.com/user-attachments/assets/a4157151-ce52-4acb-bea0-d86f6f606b02)

- Review Create → Create

- Connect to the OpenVAS VM via SSH using PowerShell (Windows) or Terminal (MacOS).

- Wait until the OpenVAS deployment completes and access the web app URL (For this example: https://172.190.177.16.c.hossted.com).

- ![image](https://github.com/user-attachments/assets/3903a7c8-7de2-4b23-b709-3b76470df5c2)

- Log in with provided credentials or try admin/admin if needed (admin/admin was used below).

- ![image](https://github.com/user-attachments/assets/a2c7ddbf-c2f1-4ea1-9683-050d931dc8d6)

- Reset the admin password to a password of your choosing in the example I will be using "incorrect".

- To change the password, you will go to the person icon at the top right of the page, then select the pencil/note icon near the top left of the page. You will then be shown a pop-up to make the change of the old password to the new password.

![image](https://github.com/user-attachments/assets/005f1b7d-52cb-4728-81c8-0c2403770b6d)


</details>
