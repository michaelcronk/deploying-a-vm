# Deploying a Windows Server Virtual Machine

## Quickly Deploy a Windows Server on a Virtual Machine in Azure using the Portal

> <sub>To get started, you first need to have a Microsoft Azure account. If you don't have one, you can create a free account [here.](https://azure.microsoft.com/en-us/free/search/?&ef_id=_k_Cj0KCQiA4NWrBhD-ARIsAFCKwWv39zVXs4ww7bj_IGmTJngZol8ZX835NOuvRgv7ygSk_rEe9lnrcGcaAg2vEALw_wcB_k_&OCID=AIDcmm5edswduu_SEM__k_Cj0KCQiA4NWrBhD-ARIsAFCKwWv39zVXs4ww7bj_IGmTJngZol8ZX835NOuvRgv7ygSk_rEe9lnrcGcaAg2vEALw_wcB_k_&gad_source=1&gclid=Cj0KCQiA4NWrBhD-ARIsAFCKwWv39zVXs4ww7bj_IGmTJngZol8ZX835NOuvRgv7ygSk_rEe9lnrcGcaAg2vEALw_wcB)</sub>

In todays project we will be creating a Windows Server (2022 Datacenter: Azure Edition) using the Azure portal.

Once you are logged into you Azure account and are at the portal home, you will first need to navigate to the "Virtual Machines" tab or click in the search bar and type "Virutal Machines". (There are many ways to create a virtual machine, any way works!)

![Alt text](<imgs/Screenshot 2024-01-04 at 7.58.28 PM.png>)

Under the "Basics" tab you will have to select the Subscription and Resource Group to create the instance in as well as a few other options that are all dependent on your specific project.

- <sup>In this example we will be using a "Windows Server 2022 Datacenter: Azure Edition" image with basic settings to keep costs down.</sup>

![Alt text](<Screenshot 2024-01-04 at 7.59.47 PM.png>)

You can select the size of the Virtual Machine you would like to run for your project, create the Username and Password, and select which Public Ports you would like to have open.

- <sup>For this example we will use the "Standard B2s" size and allow "HTTP (80)", "SSH (22)", and "RDP (3389)" since we are launching a Web Server.</sup>

![Alt text](<Screenshot 2024-01-04 at 8.00.02 PM.png>)
