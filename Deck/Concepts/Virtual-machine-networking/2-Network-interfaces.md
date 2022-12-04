##

A network interface (NIC) is the interconnection between a virtual machine and 

%

a virtual network

##

A virtual machine must have at least one NIC. A virtual machine can have more than one NIC, depending on

%

the size of the VM you create

##

You can create a VM with multiple NICs, and add or remove NICs through the lifecycle of a VM. Multiple NICs allow a VM to

%

connect to different subnets

##

Each NIC attached to a VM must exist in the same `_____` and `_____` as the VM.

%

Each NIC attached to a VM must exist in the same **location** and **subscription** as the VM.

##

Each NIC must be connected to a VNet that exists in the same Azure `_____` and `_____` as the NIC.

%

Each NIC must be connected to a VNet that exists in the same Azure **location** and **subscription** as the NIC.

##

You can change the subnet a VM is connected to after it's created. You can't change the

%

virtual network

##

Each NIC attached to a VM is assigned a MAC address that doesn't change until 

%

the VM is deleted

##

List the methods that you can use to create a network interface

%

- Azure portal
- Azure PowerShell
- Azure CLI
- Template

##

When you create a VM in the Azure portal, a network interface is

%

automatically created for you

##

When you create a VM in the Azure portal, the portal creates a VM with only one

%

NIC

##

When you create a VM in the Azure portal, if you want to create a VM with more than one NIC, you must

%

create it with a different method

##

When you create a VM with Azure PowerShell, use <u>**New-**</u>`_____` with the <u>**-**</u>`_____` parameter to provide the identifier of the public IP address that you previously created.

%

When you create a VM with Azure PowerShell, use `New-AzNetworkInterface` with the `-PublicIpAddressId` parameter to provide the identifier of the public IP address that you previously created.

##

When you create a VM with Azure CLI, to provide the identifier of the public IP address that you previously created, use <u>**az**</u>`_____` with the <u>**--**</u>`_____` parameter.

%

When you create a VM with Azure CLI, to provide the identifier of the public IP address that you previously created, use `az network nic create` with the `--public-ip-address` parameter.
