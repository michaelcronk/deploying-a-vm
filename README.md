# Deploying a Windows Server Virtual Machine

## Quickly Deploy a Windows Server on a Virtual Machine in Azure using the Portal on MacOS

<sup><strong>DISCLAIMER - This was a follow along through a sandbox enviornment using [Whizlabs](https://www.whizlabs.com/)</strong></sup>

> <sub>To get started, you first need to have a Microsoft Azure account. If you don't have one, you can create a free account [here.](https://azure.microsoft.com/en-us/free/search/?&ef_id=_k_Cj0KCQiA4NWrBhD-ARIsAFCKwWv39zVXs4ww7bj_IGmTJngZol8ZX835NOuvRgv7ygSk_rEe9lnrcGcaAg2vEALw_wcB_k_&OCID=AIDcmm5edswduu_SEM__k_Cj0KCQiA4NWrBhD-ARIsAFCKwWv39zVXs4ww7bj_IGmTJngZol8ZX835NOuvRgv7ygSk_rEe9lnrcGcaAg2vEALw_wcB_k_&gad_source=1&gclid=Cj0KCQiA4NWrBhD-ARIsAFCKwWv39zVXs4ww7bj_IGmTJngZol8ZX835NOuvRgv7ygSk_rEe9lnrcGcaAg2vEALw_wcB)</sub>

In todays project we will be creating a Windows Server (2022 Datacenter: Azure Edition) using the Azure portal.

Once you are logged into you Azure account and are at the portal home, you will first need to navigate to the "Virtual Machines" tab or click in the search bar and type "Virutal Machines". (There are many ways to create a virtual machine, any way works!)

![Alt text](<imgs/Screenshot 2024-01-04 at 7.58.28 PM.png>)

Under the "Basics" tab you will have to select the Subscription and Resource Group to create the instance in as well as a few other options that are all dependent on your specific project.

- <sup>In this example we will be using a "Windows Server 2022 Datacenter: Azure Edition" image with basic settings to keep costs down.</sup>

![Alt text](<imgs/Screenshot 2024-01-04 at 7.59.47 PM.png>)

You can select the size of the Virtual Machine you would like to run for your project, create the Username and Password, and select which Public Ports you would like to have open.

- <sup>For this example we will use the "Standard B2s" size and allow "HTTP (80)", "SSH (22)", and "RDP (3389)" since we are launching a Web Server.</sup>

![Alt text](<imgs/Screenshot 2024-01-04 at 8.00.02 PM.png>)

Under the Storage tab, select the storage you will want to use

![Alt text](<imgs/Screenshot 2024-01-04 at 8.01.11 PM.png>)

For this example I will also disable the "Boot diagnostics"

![Alt text](<imgs/Screenshot 2024-01-04 at 8.01.36 PM.png>)

When you have all your requirements selected for the VM, you can hit "Review and Create" to create the Virtual Machine.

Once the Virtual Machine is deployed, navigate to it and select the "Connect" button in the top left and download the RDP File.

![Alt text](<imgs/Screenshot 2024-01-04 at 8.04.58 PM.png>)

![Alt text](<imgs/Screenshot 2024-01-04 at 8.05.11 PM.png>)

Since I am on a Mac, I will be using the "Microsoft Remote Desktop" application to RDP into the Windows WM.

On your computer, navigate to the downloaded RDP file and run it.

- <sup><strong>NOTE:</strong> For this example it will open up a conection box using the "Microsoft Remote Desktop" application for MacOS.</sup>

![Alt text](<imgs/Screenshot 2024-01-04 at 8.07.04 PM.png>)
