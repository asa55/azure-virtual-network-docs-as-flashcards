##

You can assign these types of IP addresses to a network interface in Azure:

%

- Public IP addresses
- Private IP addresses

##

Public IP addresses are used to communicate inbound and outbound (without network address translation (NAT)) with the Internet and other Azure resources not connected to a

%

virtual network

##

Assigning a public IP address to a NIC is

%

optional

##

Public IP addresses have a nominal charge, and there's a maximum number that can be used per

%

subscription

##

`_____` IP addresses are used for communication within a virtual network, your on-premises network, and the Internet (with NAT). At least one private IP address must be assigned to a VM. 

%

**Private** IP addresses are used for communication within a virtual network, your on-premises network, and the Internet (with NAT). At least one private IP address must be assigned to a VM. 

##

You can assign public IP addresses to:

%

- Virtual machines
- Public load balancers


##

You can assign private IP address to:

%

- Virtual machines
- Internal load balancers

##

You assign IP addresses to a VM using

%

a network interface

##

There are two methods in which an IP address is given to a resource

%

- dynamic
- static

##

The default method that Azure gives IP addresses is

%

dynamic

##

An IP address is given when you `_____` a VM or `_____` VM. The IP address is released when you `_____` the VM.

%

An IP address is given when you **create** a VM or **start a stopped** VM. The IP address is released when you **stop or delete** the VM.

##

To ensure the IP address for the VM remains the same, you can set the allocation method explicitly to `_____`. In this case, an IP address is assigned `_____`. It's released only when you `_____` the VM or change its allocation method to `_____`.

%

To ensure the IP address for the VM remains the same, you can set the allocation method explicitly to **static**. In this case, an IP address is assigned **immediately**. It's released only when you **delete** the VM or change its allocation method to **dynamic**.

##

List the methods that you can use to create an IP address

%

- Azure portal
- Azure PowerShell
- Azure CLI
- Template

##

When creating an IP address in the Azure portal, by default, public IP addresses are

%

dynamic

##

Dynamic public IP addresses may change when the VM is

%

stopped or deleted

##

To guarantee that the VM always uses the same public IP address, create a `_____` public IP address.

%

To guarantee that the VM always uses the same public IP address, create a **static** public IP address.

##

By default, the Azure portal assigns a `_____` to a NIC when `_____` a VM. You can change this IP address to `_____` after the VM is created.

%

By default, the Azure portal assigns a **dynamic private IP address** to a NIC when **creating** a VM. You can change this IP address to **static** after the VM is created.

##

When creating an IP address with Azure PowerShell, you use `New-_____` with the `-_____` parameter as Dynamic or Static.

%

When creating an IP address with Azure PowerShell, you use `New-AzPublicIpAddress` with the `-AllocationMethod` parameter as Dynamic or Static.

##

When creating an IP address with Azure CLI, you use `az_____` with the `--_____` parameter as Dynamic or Static.

%

When creating an IP address with Azure CLI, you use `az network public-ip create` with the `--allocation-method` parameter as Dynamic or Static.

##

After you create a public IP address, you can associate it with a VM by assigning it to a

%

NIC

##

Azure provides a default `_____` for VMs that either aren't assigned a `_____` or are in the back-end pool of an internal basic Azure load balancer. The default `_____` mechanism provides an `_____` that isn't configurable.

%

Azure provides a default **outbound access IP** for VMs that either aren't assigned a **public IP address** or are in the back-end pool of an internal basic Azure load balancer. The default **outbound access IP** mechanism provides an **outbound IP address** that isn't configurable.


##

The default outbound access IP is disabled when

%

- a public IP address is assigned to the VM
- the VM is placed in the back-end pool of a standard load balancer, with or without outbound rules
- an Azure Virtual Network NAT gateway resource is assigned to the subnet of the VM.

##

VMs that are created by virtual machine scale sets in flexible orchestration mode don't have default

%

outbound access
