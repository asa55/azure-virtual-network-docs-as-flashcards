##

Virtual Network NAT (network address translation) simplifies outbound-only Internet connectivity for

%

virtual networks

##

When Virtual Network NAT is configured on a subnet, all outbound connectivity uses your specified

%

static public IP addresses

##

With Azure Virtual Network NAT, outbound connectivity is possible without load balancer or public IP addresses directly attached to

%

virtual machines

##

Azure Virtual Network NAT is fully `_____` and highly resilient.

%

Azure Virtual Network NAT is fully **managed** and highly resilient.

##

Outbound connectivity can be defined for each subnet with `_____`. Multiple subnets within the same virtual network can have different `_____`. A subnet is configured by specifying which `_____` gateway resource to use. All UDP and TCP outbound flows from any virtual machine instance will use `_____`. `_____` is compatible with standard SKU public IP address resources or public IP prefix resources or a combination of both. You can use a public IP prefix directly or distribute the public IP addresses of the prefix across multiple `_____` gateway resources. `_____` will groom all traffic to the range of IP addresses of the prefix. Any IP filtering of your deployments is easier.

%

Outbound connectivity can be defined for each subnet with **NAT**. Multiple subnets within the same virtual network can have different **NATs**. A subnet is configured by specifying which **NAT** gateway resource to use. All UDP and TCP outbound flows from any virtual machine instance will use **NAT**. **NAT** is compatible with standard SKU public IP address resources or public IP prefix resources or a combination of both. You can use a public IP prefix directly or distribute the public IP addresses of the prefix across multiple **NAT** gateway resources. **NAT** will groom all traffic to the range of IP addresses of the prefix. Any IP filtering of your deployments is easier.

##

All outbound traffic for the subnet is processed by `_____` automatically without any customer configuration. User-defined routes aren't necessary. `_____` takes precedence over other outbound scenarios and replaces the default Internet destination of a subnet.

%

All outbound traffic for the subnet is processed by **NAT** automatically without any customer configuration. User-defined routes aren't necessary. **NAT** takes precedence over other outbound scenarios and replaces the default Internet destination of a subnet.

##

Virtual machines created by Virtual machine scale sets Flexible Orchestration mode don't have default outbound access. `_____` is the recommended outbound access method for Virtual machine scale sets Flexible Orchestration Mode.

%

Virtual machines created by Virtual machine scale sets Flexible Orchestration mode don't have default outbound access. **Virtual network NAT** is the recommended outbound access method for Virtual machine scale sets Flexible Orchestration Mode.

##

List the methods that you can use to create a NAT gateway resource

%

- Azure portal
- Azure PowerShell
- Azure CLI
- Template

##

When creating a NAT gateway resource in the Azure portal, Azure creates a `_____`, `_____`, `_____`, NAT gateway, and a `_____` to test the NAT gateway resource.

%

When creating a NAT gateway resource in the Azure portal, Azure creates a **VNet**, **subnet**, **public IP**, NAT gateway, and a **VM** to test the NAT gateway resource.

##

When creating a NAT gateway resource with Azure PowerShell, use `New-_____` to create a NAT gateway resource. Creates a virtual network, subnet, public IP, NAT gateway, and a virtual machine to test the NAT gateway resource.

%

When creating a NAT gateway resource with Azure PowerShell, use `New-AzNatGateway` to create a NAT gateway resource. Creates a virtual network, subnet, public IP, NAT gateway, and a virtual machine to test the NAT gateway resource.

##

When creating a NAT gateway resource with Azure CLI, use `az_____` to create a NAT gateway resource. Creates a virtual network, subnet, public IP, NAT gateway, and a virtual machine to test the NAT gateway resource.

%

When creating a NAT gateway resource with Azure CLI, use `az network nat gateway create` to create a NAT gateway resource. Creates a virtual network, subnet, public IP, NAT gateway, and a virtual machine to test the NAT gateway resource.
