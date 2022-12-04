##

Azure Load Balancer can be configured to balance incoming Internet traffic to `_____` or balance traffic between `_____` in a VNet. A load balancer can also balance traffic between on-premises computers and `_____` in a cross-premises network, or forward external traffic to a specific `_____`.

%

Azure Load Balancer can be configured to balance incoming Internet traffic to **VMs** or balance traffic between **VMs** in a VNet. A load balancer can also balance traffic between on-premises computers and **VMs** in a cross-premises network, or forward external traffic to a specific **VM**.

##

The load balancer maps incoming and outgoing traffic between:

%

- The public IP address and port on the load balancer.
- The private IP address and port of the VM.

##

When you create a load balancer, you must also consider these configuration elements:

%

- Front-end IP configuration
- Back-end address pool
- Port Forwarding
- Load balancer rules
- Probes
- Outbound rules

##

Load balancer front-end IP configuration: A load balancer can include one or more front-end IP addresses. These IP addresses serve as ingress for 

%

the traffic

##

Load balancer back-end address pool: IP addresses that are associated with the NIC to which

%

load is distributed

##

Load balancer Port Forwarding: Defines how inbound traffic flows through the front-end IP and distributed to the back-end IP using inbound

%

NAT rules

##

Load balancer rules: Maps a given `_____` IP and port combination to a set of `_____` IP addresses and port combination. A single load balancer can have multiple load-balancing rules.

%

Load balancer rules: Maps a given **front-end** IP and port combination to a set of **back-end** IP addresses and port combination. A single load balancer can have multiple load-balancing rules.

##

Load balancer Probes: Monitors the health of VMs. When a probe fails to respond, the load balancer stops sending new connections to the unhealthy VM. The existing connections aren't affected, and new connections are sent to

%

healthy VMs

##

Load balancer outbound rules: An outbound rule configures outbound Network Address Translation (NAT) for all virtual machines or instances identified by the backend pool of your Standard Load Balancer to be translated to

%

the frontend

##

List the methods that you can use to create an internet-facing load balancer

%

- Azure portal
- Azure PowerShell
- Azure CLI
- Template

##

When creating an internet-facing load balancer with Azure PowerShell, to provide the identifier of the public IP address that you previously created, use `New-_____` with the `-_____` parameter. Use `New-_____` to create the configuration of the back-end address pool. Use `New-_____` to create inbound NAT rules associated with the front-end IP configuration that you created. Use `New-_____` to create the probes that you need. Use `New-_____` to create the load balancer configuration. Use `New-_____` to create the load balancer.

%

When creating an internet-facing load balancer with Azure PowerShell, to provide the identifier of the public IP address that you previously created, use `New-AzLoadBalancerFrontendIpConfig` with the `-PublicIpAddress` parameter. Use `New-AzLoadBalancerBackendAddressPoolConfig` to create the configuration of the back-end address pool. Use `New-AzLoadBalancerInboundNatRuleConfig` to create inbound NAT rules associated with the front-end IP configuration that you created. Use `New-AzLoadBalancerProbeConfig` to create the probes that you need. Use `New-AzLoadBalancerRuleConfig` to create the load balancer configuration. Use `New-AzLoadBalancer` to create the load balancer.

##

When creating an internet-facing load balancer with Azure CLI, use `az_____` to create the initial load balancer configuration. Use `az_____` to add the public IP address that you previously created. Use `az_____` to add the configuration of the back-end address pool. Use `az_____` to add NAT rules. Use `az_____` to add the load balancer rules. Use `az_____` to add the probes.

%

When creating an internet-facing load balancer with Azure CLI, use `az network lb create` to create the initial load balancer configuration. Use `az network lb frontend-ip create` to add the public IP address that you previously created. Use `az network lb address-pool create` to add the configuration of the back-end address pool. Use `az network lb inbound-nat-rule create` to add NAT rules. Use `az network lb rule create` to add the load balancer rules. Use `az network lb probe create` to add the probes.

##

List the methods that you can use to create an internal load balancer

%

- Azure portal
- Azure PowerShell
- Azure CLI
- Template

##

When creating an internet-facing load balancer with Azure PowerShell, to provide a private IP address in the network subnet, use `New-_____` with the `-_____` parameter. Use `New-_____` to create the configuration of the back-end address pool. Use `New-_____` to create inbound NAT rules associated with the front-end IP configuration that you created. Use `New-_____` to create the probes that you need. Use `New-_____` to create the load balancer configuration. Use `New-_____` to create the load balancer.

%

When creating an internet-facing load balancer with Azure PowerShell, to provide a private IP address in the network subnet, use `New-AzLoadBalancerFrontendIpConfig` with the `-PrivateIpAddress` parameter. Use `New-AzLoadBalancerBackendAddressPoolConfig` to create the configuration of the back-end address pool. Use `New-AzLoadBalancerInboundNatRuleConfig` to create inbound NAT rules associated with the front-end IP configuration that you created. Use `New-AzLoadBalancerProbeConfig` to create the probes that you need. Use `New-AzLoadBalancerRuleConfig` to create the load balancer configuration. Use `New-AzLoadBalancer` to create the load balancer.

##

When creating an internet-facing load balancer with Azure CLI, use the `az_____` command to create the initial load balancer configuration. To define the private IP address, use `az_____` with the `--_____` parameter. Use `az_____` to add the configuration of the back-end address pool. Use `az_____` to add NAT rules. Use `az_____` to add the load balancer rules. Use `_____` to add the probes.

%

When creating an internet-facing load balancer with Azure CLI, use the `az network lb create` command to create the initial load balancer configuration. To define the private IP address, use `az network lb frontend-ip create` with the `--private-ip-address` parameter. Use `az network lb address-pool create` to add the configuration of the back-end address pool. Use `az network lb inbound-nat-rule create` to add NAT rules. Use `az network lb rule create` to add the load balancer rules. Use `az network lb probe create` to add the probes.
