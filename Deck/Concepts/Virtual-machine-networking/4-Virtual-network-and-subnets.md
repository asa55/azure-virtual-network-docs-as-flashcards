##

Each NIC in a VM is connected to one 
`_____` in one `_____`.

%

Each NIC in a VM is connected to one 
**subnet** in one **virtual network**.

##

NICs connected to subnets (same or different) within a virtual network can communicate with each other without any extra 

%

configuration

##

When you set up a VNet, select address ranges that don't overlap if the virtual network is connected to

%

- other virtual networks or
- on-premises networks

##

When you set up a VNet, the IP addresses are private and can't be accessed from

%

the Internet

##

When you set up a VNet, Azure treats any address range as part of the private virtual network IP address space. The address range is only reachable 

%

- within the virtual network
- within interconnected virtual networks
- from your on-premises location

##

If you work within an organization in which someone else is responsible for the internal networks, talk to that person before selecting your `_____`. Ensure there's no overlap in the `_____`. Communicate to them the `_____` you want to use so they don't try to use the same range of IP addresses.

%

If you work within an organization in which someone else is responsible for the internal networks, talk to that person before selecting your **address space**. Ensure there's no overlap in the **address space**. Communicate to them the **address space** you want to use so they don't try to use the same range of IP addresses.

##

There aren't security boundaries by default between subnets. Virtual machines in each of these subnets can communicate. If your deployment requires security boundaries, use `_____`, which control the traffic flow to and from subnets and to and from VMs.

%

There aren't security boundaries by default between subnets. Virtual machines in each of these subnets can communicate. If your deployment requires security boundaries, use **Network Security Groups (NSGs)**, which control the traffic flow to and from subnets and to and from VMs.

##

List the methods that you can use to create a virtual network and subnets

%

- Azure portal
- Azure PowerShell
- Azure CLI
- Template

##

If you let Azure create a virtual network when you create a VM in Azure portal, the name is a combination of

%

- the resource group name that contains the VNet 
- and `-vnet`

##

If you let Azure create a virtual network when you create a VM in Azure portal, the address space is `_____`, the required subnet name is `_____`, and the subnet address range is `_____`.

%

If you let Azure create a virtual network when you create a VM in Azure portal, the address space is `10.0.0.0/24`, the required subnet name is `default`, and the subnet address range is `10.0.0.0/24`.

##

When creating a VNet and subnets in Azure PowerShell, you use `New-_____` and `New-_____` to create a subnet and a virtual network. You can also use `Add-_____` to add a subnet to an existing virtual network.

%

When creating a VNet and subnets with Azure PowerShell, you use `New-AzVirtualNetworkSubnetConfig` and `New-AzVirtualNetwork` to create a subnet and a virtual network. You can also use `Add-AzVirtualNetworkSubnetConfig` to add a subnet to an existing virtual network.

##

When creating a VNet and subnets with Azure CLI, the subnet and the virtual network are created at the same time. Provide a `--_____` parameter to `az_____` with the subnet name.

%

When creating a VNet and subnets with Azure CLI, the subnet and the virtual network are created at the same time. Provide a `--subnet-name` parameter to `az network vnet create` with the subnet name.
