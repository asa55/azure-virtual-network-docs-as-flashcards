##

A network security group (NSG) contains a list of Access Control List (ACL) rules that allow or deny network traffic to 

%

- subnets
- NICs
- or both

##

NSGs can be associated with either 

%

- subnets or
- individual NICs connected to a subnet

##

When an NSG is associated with a subnet, the ACL rules apply to all the VMs in 

%

that subnet

##

Traffic to an individual NIC can be restricted by associating an NSG directly to

%

a NIC

##

NSGs contain two sets of rules, inbound and outbound. The priority for a rule must be unique within each set.

Each rule has properties of:

%

- Protocol
- Source and destination port ranges
- Address prefixes
- Direction of traffic
- Priority
- Access type

##

All NSGs contain a set of default rules. The default rules cannot be `_____`. They're assigned the lowest `_____` and can't be overridden by the rules that `_____`.

%

All NSGs contain a set of default rules. The default rules cannot be **deleted**. They're assigned the lowest **priority** and can't be overridden by the rules that **you create**.

##

When you associate an NSG to a NIC, the network access rules in the NSG are applied only to 

%

that NIC

##

If an NSG is applied to a single NIC on a multi-NIC VM, it doesn't affect traffic to

%

the other NICs

##

You can associate different NSGs to a `_____` (or `_____`, depending on the deployment model) and the subnet that a `_____` or `_____` is bound to.

%

You can associate different NSGs to a **NIC** (or **VM**, depending on the deployment model) and the subnet that a **NIC** or **VM** is bound to.

##

In Network Security Groups, priority is given based on the `_____` of traffic.

%

In Network Security Groups, priority is given based on the **direction** of traffic.

##

Be sure to plan your `_____` when you plan your virtual machines and virtual network.

%

Be sure to plan your **NSGs** when you plan your virtual machines and virtual network.

##

List the methods that you can use to create a network security group

%

- Azure portal
- Azure PowerShell
- Azure CLI
- Template

##

When you create a VM in the Azure portal, an NSG is automatically created and associated to the NIC the portal creates. The name of the NSG is a combination of the `_____` and `_____`.
This NSG contains one inbound rule:
- With a priority of `_____`.
- The service set to `_____`.
- The protocol set to `_____`.
- The port set to `_____`.
- The action set to `_____`.
If you want to allow any other inbound traffic to the VM, create another `_____`.

%

When you create a VM in the Azure portal, an NSG is automatically created and associated to the NIC the portal creates. The name of the NSG is a combination of the **name of the VM** and `-nsg`.
This NSG contains one inbound rule:
- With a priority of `1000`.
- The service set to `RDP`.
- The protocol set to `TCP`.
- The port set to `3389`.
- The action set to `Allow`.
If you want to allow any other inbound traffic to the VM, create another **rule or rules**.

##

When creating a NSG with Azure PowerShell, use `New-_____` and provide the required rule information. Use `New-_____` to create the NSG. Use `Set-_____` to configure the NSG for the subnet. Use `Set-_____` to add the NSG to the virtual network.

%

When creating a Network Security Group (NSG) with Azure PowerShell, use `New-AzNetworkSecurityRuleConfig` and provide the required rule information. Use `New-AzNetworkSecurityGroup` to create the NSG. Use `Set-AzVirtualNetworkSubnetConfig` to configure the NSG for the subnet. Use `Set-AzVirtualNetwork` to add the NSG to the virtual network.

##

When creating a Network Security Group (NSG) with Azure CLI, use `az_____` to initially create the NSG. Use `az_____` to add rules to the NSG. Use `az_____` to add the NSG to the subnet.

%

When creating a Network Security Group (NSG) with Azure CLI, use `az network nsg create` to initially create the NSG. Use `az network nsg rule create` to add rules to the NSG. Use `az network vnet subnet update` to add the NSG to the subnet.
