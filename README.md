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

</br>

<h3>Step 2: Creating an Azure Resource Group(RG)</h3>

 - Using the Azure Search Bar at the top of the Azure Portal, search “Resource Groups” and press Enter twice.
 - Press “Create” at the top of the RG overview page.
 - Choose a name for your RG.
 - Select the region you would like your RG to be hosted in.
 - Click “Review + Create” at the bottom left of the “Create a Resource Group” page.
 - Then click  “Create.”
 - Wait for the resources to be made on the back end.

</br>

<h3>Step 3: Creating an Azure Virtual Machine(VM)</h3>

 - Using the Azure Search Bar again, search “Virtual Machines” and press Enter twice.
 - Press “Create” followed by “Virtual Machine” at the top of the VM overview page.
 - Input the name of the RG you just made.
 - Ensure the selected region matches your RG’s region.
 - Choose a name for your VM.
 - Choose “Windows 11 Pro, version 25H2 - x64 Gen2” for the “Image.”
 - Choose “Standard_D2s_v3 - 2 vcpus, 8 GiB memory” for the “Size”
 - If you receive an error message stating that the zone is not available, select a suggested zone. 
 - Choose a Username and Password for the Administrator Account.
 - In the Licensing section, read the agreement and check the box.
 - In the bottom left, click “Next” twice to get to the Networking section.
 - Click “Edit virtual network” under the “Virtual Network” name input box.
 - Choose a name for your new Virtual Network(vnet) and click “Save”.
 - In the bottom left, click “Review + Create”.
 - Wait for the validation process to finish, then click “Create”.
 - Wait for the resources to be made on the back end.

</br>

<h3>Step 4: Log in to the Virtual Machine</h3>

 - Return to the VM overview page, open the VM you just created
 - On the “Overview” tab, locate “Primary NIC public IP” in the “Essentials” blade.
 - Copy the IP address to your clipboard.
 - Open the Windows Start menu, type “RDP,” and press Enter.
 - Put the VM’s public IP address into the “Computer” section and press “Connect”.
 - Enter the login credentials for the admin account you created for the VM and press Enter.
 - If the Remote Desktop Connection warning appears, click “Yes”.
 - Once the VM is done booting up, select your desired setup for the initial settings and press “Accept.”

</br>

<h3>Congrats! You’ve successfully created and logged into an Azure Virtual Machine.</h3>




