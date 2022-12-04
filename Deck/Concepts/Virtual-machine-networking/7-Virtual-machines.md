##

Virtual machines can be created in the same virtual network and they can connect to each other using

%

private IP addresses

##

Virtual machines can connect if they're in different `_____`. They connect without the need to configure a `_____` or use `_____`.

%

Virtual machines can connect if they're in different **subnets**. They connect without the need to configure a **gateway** or use **public IP addresses**.

##

To put VMs into a virtual network, you create the virtual network. As you create each VM, you assign it to the virtual network and subnet. Virtual machines acquire their network settings during

%

deployment or startup

##

Virtual machines are assigned an IP address when they're

%

deployed

##

When you deploy multiple VMs into a virtual network or subnet, they're assigned IP addresses as they

%

boot up

##

You can also assign a `_____` IP to a VM. If you assign a `_____` IP, you should consider using a specific subnet to avoid accidentally reusing a `_____` IP for another VM.

%

You can also assign a **static** IP to a VM. If you assign a **static** IP, you should consider using a specific subnet to avoid accidentally reusing a **static** IP for another VM.

##

If you create a VM and later want to migrate it into a virtual network, it isn't a simple configuration change. `_____` the VM into the virtual network. The easiest way to `_____` is to delete the VM, but not any disks attached to it, and then re-create the VM using the original disks in the virtual network.

%

If you create a VM and later want to migrate it into a virtual network, it isn't a simple configuration change. **Redeploy** the VM into the virtual network. The easiest way to **redeploy** is to delete the VM, but not any disks attached to it, and then re-create the VM using the original disks in the virtual network.

##

List the methods that you can use to create a VM in a VNet

%

- Azure portal
- Azure PowerShell
- Azure CLI
- Template

##

When creating a VM in a VNet in the Azure portal, Azure uses default network settings to create a VM with a single NIC. To create a VM with multiple NICs, you must

%

use a different method

##

When creating a VM in a VNet with Azure PowerShell, use <u>**Add-**</u>`_____` to add a previously created NIC to the VM configuration.

%

When creating a VM in a VNet with Azure PowerShell, use `Add-AzVMNetworkInterface` to add a previously created NIC to the VM configuration.
