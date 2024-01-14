# Deploying a Windows Server Virtual Machine

## Quickly Deploy a Windows Server on a Virtual Machine in Azure using the Portal (on MacOS)

<sup><strong>DISCLAIMER</strong> - This was a follow along sandbox enviornment using [Whizlabs](https://www.whizlabs.com/)</sup>

> <sub>To get started, you first need to have a Microsoft Azure account. If you don't have one, you can create a free account [here.](https://azure.microsoft.com/en-us/free/search/?&ef_id=_k_Cj0KCQiA4NWrBhD-ARIsAFCKwWv39zVXs4ww7bj_IGmTJngZol8ZX835NOuvRgv7ygSk_rEe9lnrcGcaAg2vEALw_wcB_k_&OCID=AIDcmm5edswduu_SEM__k_Cj0KCQiA4NWrBhD-ARIsAFCKwWv39zVXs4ww7bj_IGmTJngZol8ZX835NOuvRgv7ygSk_rEe9lnrcGcaAg2vEALw_wcB_k_&gad_source=1&gclid=Cj0KCQiA4NWrBhD-ARIsAFCKwWv39zVXs4ww7bj_IGmTJngZol8ZX835NOuvRgv7ygSk_rEe9lnrcGcaAg2vEALw_wcB)</sub>

In todays project we will be creating a Windows Server (2022 Datacenter: Azure Edition) using the Azure portal.

Once you are logged into you Azure account and are at the portal home, you will first need to navigate to the "Virtual Machines" tab or click in the search bar and type "Virutal Machines". (There are many ways to create a virtual machine, any way works!)

![Alt text](<imgs/Screenshot 2024-01-04 at 7.58.28 PM.png>)

Under the "Basics" tab you will have to select the Subscription and Resource Group to create the instance in as well as a few other options that are all dependent on your specific project.

- <sup>For this example we will be using a "Windows Server 2022 Datacenter: Azure Edition" image with basic settings to keep costs down.</sup>

![Alt text](<imgs/Screenshot 2024-01-04 at 7.59.47 PM.png>)

You can select the size of the Virtual Machine you would like to run for your project, create the Username and Password, and select which Public Ports you would like to have open.

- <sup>For this example we will use the "Standard B2s" size and allow "HTTP (80)", "SSH (22)", and "RDP (3389)" since we are launching a Web Server. I didn't add any "Netowrk Security Group" to the public ports in this example, but if you are going to run a production VM then consider adding some security to the public ports. If you want to learn more about port security, check out [this article.](https://learn.microsoft.com/en-us/azure/virtual-network/network-security-groups-overview)</sup>

![Alt text](<imgs/Screenshot 2024-01-04 at 8.00.02 PM.png>)

Under the Storage tab, select the storage you will want to use.

![Alt text](<imgs/Screenshot 2024-01-04 at 8.01.11 PM.png>)

In this example I will also disable the "Boot diagnostics".

![Alt text](<imgs/Screenshot 2024-01-04 at 8.01.36 PM.png>)

When you have all your requirements selected for the VM, you can hit "Review and Create" to create the Virtual Machine.

Once the Virtual Machine is deployed, navigate to it and select the "Connect" button in the top left and download the RDP File.

![Alt text](<imgs/Screenshot 2024-01-04 at 8.04.58 PM.png>)

![Alt text](<imgs/Screenshot 2024-01-04 at 8.05.11 PM.png>)

Since I am on a Mac, I will be using the "Microsoft Remote Desktop" application to connect to the Windows WM.

On your computer, navigate to the downloaded RDP file and run it.

- <sup><strong>NOTE:</strong> For this example it will open up a conection box using the "Microsoft Remote Desktop" application for MacOS.</sup>

![Alt text](<imgs/Screenshot 2024-01-04 at 8.07.04 PM.png>)

Now that we are logged into the Windows VM, you can see the Server Manager application and proceed to manage your server how you see fit.

![Alt text](<imgs/Screenshot 2024-01-04 at 8.20.14 PM.png>)

Once you are done you can disconnect from the VM and either clean up your resources so you don't accumulate any more costs or keep the server running for your needs.

For this example we will clean up our resources since we only used this VM for our example project.

We will head into the Azure portal, find our resource group that contains all of our VMs resources and click into the resource group.

From here we have two options:

1. Delete the resource group entirely.

2. Delete the resources inside of the resource group.

We will be deleting the resources inside the group for this project.

Once inside the resource group you can select all the resources by clicking the "name" checkbox and then clicking "delete", as shown below.

![Alt text](<imgs/Screenshot 2024-01-04 at 8.21.32 PM.png>)

When prompted, type "delete" and click the delete button.

![Alt text](<imgs/Screenshot 2024-01-04 at 8.21.59 PM.png>)

Now wait until you see that all your resources have been deleted without an error.

With that you have now created a VM, connected to the VM, and deleted all the VMs resources within this project.

If you have any questions, message me on Discord, Instagram or comment on this repo. Thank you for following along!
