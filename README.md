## Azure Network Practice
This repository was created as a journal where I can keep notes and small projects I made with Azure Cloud.  
**31.03** - I set up a base for the network: VNet, subnets, route table, and a virtual machine.  

### Project Diagram  
![Project Diagram](https://github.com/Jaksa1703/Azure-900-Practice/blob/main/Vnet/Concept.png)  

### Resource Group  
First, I had to create a resource group - **"Azure-practice-vnet"**  
![Resource Group](https://github.com/Jaksa1703/Azure-900-Practice/blob/main/Vnet/Resource_group.png)  

### Virtual Network (VNet)  
Next, I created a virtual network so my machines could communicate and access the internet.  
![VNet Creation](https://github.com/Jaksa1703/Azure-900-Practice/blob/main/Vnet/Vnet_creation.png)  

### Subnet Configuration  
I decided to separate the network into two subnets: **private** and **public**.  

**Private Subnet:**  
![Private Subnet](https://github.com/Jaksa1703/Azure-900-Practice/blob/main/Vnet/Private_subnet.png)  

**Public Subnet:**  
![Public Subnet](https://github.com/Jaksa1703/Azure-900-Practice/blob/main/Vnet/Public_subnet.png)  

I wanted only one VM to be able to connect to the internet, so I divided them into two separate subnets.  

**List of Associated Subnets:**  
![Subnets List](https://github.com/Jaksa1703/Azure-900-Practice/blob/main/Vnet/list_of_associated_subnets.png)  

**Public Internet Access Configuration:**  
![Public Internet Access](https://github.com/Jaksa1703/Azure-900-Practice/blob/main/Vnet/public_internet_access.png)  

### Virtual Machine (VM) Setup  
Once my subnets were ready, I created a virtual machine in the **public** subnet. I chose **Ubuntu Server LTS 24.04** as the OS to minimize resource usage.  

**Public VM Access Configuration:**  
![Public VM Access](https://github.com/Jaksa1703/Azure-900-Practice/blob/main/Vnet/Public_VM_access.png)  

I was able to connect to my Ubuntu machine via **SSH**.  

**SSH Connection:**  
![SSH Connection](https://github.com/Jaksa1703/Azure-900-Practice/blob/main/Vnet/public_vm.png)  

### Next Steps  
Later, I plan to add:  
✅ A second VM in the **private** subnet.  
✅ A **Network Security Group (NSG)** for security management.  
