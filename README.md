<h1>Azure: VM Deployment and Configuration</h1>
This tutorial outlines the steps required to setup and connect to a Virtual Machine using Microsoft Azure.

 <h2>Environments and Technologies Used</h2>

  - Google Chrome (Web Browser)
  - Microsoft Azure Portal  
  - Microsoft Azure (Virtual Machines)
  - Remote Desktop
 
 <h2>Operating Systems Used </h2>

 - Windows 10 Home (22H2)
 - Windows 11 Pro (25H2)
 
 <h2>List of Prerequisites</h2>

 - Microsoft Azure Tenant
 - Microsoft Azure Subscription

<h2>Setup Procedure</h2>

<h3>Step 1: Enter the Azure Portal</h3>

 - Open your Web Browser of choice.
 - Log in to the Azure Portal at: https://portal.azure.com/
   > <img width="50%" height="50%" alt="Azure Portal Home" src="https://github.com/user-attachments/assets/10261bbd-adbf-485f-a842-b0a54a384bf9" />



</br>

<h3>Step 2: Creating an Azure Resource Group(RG)</h3>

 - Using the Azure Search Bar at the top of the Azure Portal, search “Resource Groups” and press Enter twice.
   > <img width="50%" height="50%" alt="Azure Portal Search" src="https://github.com/user-attachments/assets/4e4b88ae-9ae7-4c7d-abb9-f278fa71f09c" />
 - Press “Create” at the top of the RG overview page.
   > <img width="50%" height="50%" alt="RG List" src="https://github.com/user-attachments/assets/b5b89949-951a-4b4b-b2d6-29f2239eceb3" />
 - Choose a name for your RG.
 - Select the region you would like your RG to be hosted in.
 - Click “Review + Create” at the bottom left of the “Create a Resource Group” page.
   > <img width="50%" height="50%" alt="RG Creation" src="https://github.com/user-attachments/assets/a255cb02-432f-402d-87bb-da068eaa3107" />
 - Then click  “Create.”
 - Wait for the resources to be made on the back end.

</br>

<h3>Step 3: Creating an Azure Virtual Machine(VM)</h3>

 - Using the Azure Search Bar again, search “Virtual Machines” and press Enter twice.
 - Press “Create” followed by “Virtual Machine” at the top of the VM overview page.
   > <img width="50%" height="50%" alt="VM List" src="https://github.com/user-attachments/assets/54fcc42b-2063-4469-b491-6ca8bbe686d8" />
 - Input the name of the RG you just made.
 - Ensure the selected region matches your RG’s region.
 - Choose a name for your VM.
   > <img width="50%" height="50%" alt="VM Creation 1" src="https://github.com/user-attachments/assets/735a1da9-fc6d-4cc0-bb9b-8916b9d08ce7" />
 - Choose “Windows 11 Pro, version 25H2 - x64 Gen2” for the “Image.”
 - Choose “Standard_D2s_v3 - 2 vcpus, 8 GiB memory” for the “Size”
 - If you receive an error message stating that the zone is not available, select a suggested zone.
   > <img width="50%" height="50%" alt="VM Creation 2" src="https://github.com/user-attachments/assets/83a25911-5bba-4041-8916-f5c57b078b6f" />
 - Choose a Username and Password for the Administrator Account.
 - In the Licensing section, read the agreement and check the box.
   > <img width="50%" height="50%" alt="VM Creation 3" src="https://github.com/user-attachments/assets/f0bee495-54f5-4aea-aaad-14bdb2d97553" />
 - In the bottom left, click “Next” twice to get to the Networking section.
 - Click “Edit virtual network” under the “Virtual Network” name input box.
 - Choose a name for your new Virtual Network(vnet) and click “Save”.
   > <img width="50%" height="50%" alt="VM Creation 4" src="https://github.com/user-attachments/assets/420c46f9-2172-4db4-8194-cf8f8bb69bed" />
 - In the bottom left, click “Review + Create”.
 - Wait for the validation process to finish, then click “Create”.
 - Wait for the resources to be made on the back end.

</br>

<h3>Step 4: Log in to the Virtual Machine</h3>

 - Return to the VM overview page, open the VM you just created
 - On the “Overview” tab, locate “Primary NIC public IP” in the “Essentials” blade.
   > <img width="50%" height="50%" alt="VM Overview Tab" src="https://github.com/user-attachments/assets/1d9b127a-f515-4498-ac14-4ff777ef7f09" />
 - Copy the IP address to your clipboard.
 - Open the Windows Start menu, type “RDP,” and press Enter.
 - Put the VM’s public IP address into the “Computer” section and press “Connect”.
   > <img width="50%" height="50%" alt="RDP Connection" src="https://github.com/user-attachments/assets/c0f5a609-f35f-4892-aa32-c94d4361dd6a" />
 - Enter the login credentials for the admin account you created for the VM and press Enter.
 - If the Remote Desktop Connection warning appears, click “Yes”.
 - Once the VM is done booting up, select your desired setup for the initial settings and press “Accept.”

</br>

<h3>Congrats! You’ve successfully created and logged into an Azure Virtual Machine.</h3>
  > <img width="50%" height="50%" alt="VM Desktop" src="https://github.com/user-attachments/assets/7abb494e-3aa8-45d7-a394-5a878c974e42" />





