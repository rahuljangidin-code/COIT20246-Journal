# Week 08 – Cloud Computing

---

## Task 1 – Knowledge Test

The Week 08 knowledge test was completed during the tutorial as required.

---

## Task 3 – Azure Resource Creation

Several Azure resources were created using Microsoft Learn On Demand.

### Azure Resources Created

- **Resource Group**  
  Used to logically organise and manage all Azure resources related to the virtual machine.

- **Virtual Network (VNet)**  
  Provides a private network environment for Azure resources to communicate securely.

- **Subnet**  
  Divides the virtual network into smaller address spaces for better network management.

- **Network Interface (NIC)**  
  Connects the virtual machine to the virtual network.

- **Public IP Address**  
  Allows external access to the virtual machine from the internet.

- **Network Security Group (NSG)**  
  Controls inbound and outbound network traffic using security rules.

Each resource plays a role in enabling secure deployment and access to cloud-based services.

---

## Task 4 – Azure Virtual Machine and Web Access

An Ubuntu virtual machine was created in Azure and configured to host a web server.

### Azure Commands Used

The following Azure CLI commands were used to create the virtual machine and install the web server:

```bash
az group create --name myResourceGroup --location australiaeast

az vm create \
  --resource-group myResourceGroup \
  --name myVM \
  --image UbuntuLTS \
  --admin-username azureuser \
  --generate-ssh-keys

az vm open-port \
  --resource-group myResourceGroup \
  --name myVM \
  --port 80

az vm run-command invoke \
  --resource-group myResourceGroup \
  --name myVM \
  --command-id RunShellScript \
  --scripts "sudo apt update && sudo apt install nginx -y"
