##

The abbreviation for Azure Virtual Network is

%

VNet

##

Azure Virtual Network the fundamental building block of

%

your private network in Azure

##

Azure virtual network enables Azure resources to securely communicate with

%

- Each other
- The internet
- On-premises networks

##

VNets are similar to

%

a traditional network that you'd operate in your own data center

##

VNet offers additional benefits of Azure's infrastructure over a network you'd operate in your own data center such as

%

- Scale
- Availability
- Isolation

##

Key scenarios you can accomplish with a virtual network include

%

- Communication of Azure resources with the internet
- Communication between Azure resources
- Communication with on-premises resources
- Filtering network traffic
- Routing network traffic
- Integration with Azure resources

##

By default, all resources in a VNet can communicate outbound to

%

the internet

##

To communicate inbound from the internet to a resource in a VNet, assign

%

a public IP address or a public Load Balancer

##

To manage outbound connections from a VNet to the internet, you can use

%

a public IP address or public Load Balancer

##

Outbound connectivity to the internet when using only an internal Standard Load Balancer is not available until you define how you want outbound connections to work with:

%

- An instance-level public IP or
- a public Load Balancer

##

Azure resources can communicate securely with each other through

%

- a VNet
- a VNet service endpoint
- VNet Peering

##

You can connect your on-premises resources to a VNet with

%

- Point-to-site virtual private network (VPN)
- Site-to-site VPN
- Azure ExpressRoute

##

Connecting on-premises resources to a VNet using point-to-site VPN means establishing a connection between a VNet and a `_____` in your network.

%

Connecting on-premises resources to a VNet using point-to-site VPN means establishing a connection between a VNet and a **single computer** in your network.

##

When connecting on-premises resources to a VNet using point-to-site VPN, each computer that wants to establish connectivity with a VNet must

%

configure its connection

##

When connecting on-premises resources to a VNet using point-to-site VPN, communication between your computer and a VNet is sent through an encrypted tunnel over

%

the internet

##

Connecting on-premises resources to a VNet using point-to-site VPN requires little or no changes to existing network, making point-to-site VPN well suited for

%

- Developers
- Getting started with Azure

##

Connecting on-premises resources to a VNet using site-to-site VPN means establishing a connection between your on-premises VPN device and an Azure VPN Gateway deployed within

%

a VNet

##

Connecting on-premises resources to a VNet using site-to-site VPN enables any on-premises resource that you authorize to access

%

a VNet

##

When connecting on-premises resources to a VNet using site-to-site VPN, communication between your on-premises VPN device and an Azure VPN gateway is sent through an encrypted tunnel over

%

the internet

##

Connecting on-premises resources to a VNet using Azure ExpressRoute means establishing a connection between your network and Azure, through

%

an ExpressRoute partner

##

When connecting on-premises resources to a VNet using Azure ExpressRoute, the connection is private. Traffic does not go over

%

the internet

##

You can filter network traffic between subnets using

%

- Network security groups
- Network virtual appliances

##

Network security groups (and application security groups) can contain multiple inbound and outbound security rules that enable you to filter traffic to and from resources by

%

- source IP address
- destination IP address
- port
- protocol

##

A Network Virtual Appliance (NVA) is a VM that performs a network function, such as

%

- a firewall
- a WAN optimization
- or other network function

##

A list of available network virtual appliances that you can deploy in a virtual network can be found in

%

Azure Marketplace

##

By default, Azure routes traffic between

%

- Subnets
- Connected VNets
- Connected on-premises networks
- the internet

##

To override the default routes created by Azure, you can use

%

- Custom route tables
- Border gateway protocol (BGP) routes
  - (The BGP routes option only applies if you connect your virtual network to your on-premises network using Azure VPN Gateway or ExpressRoute)

##

Integrating Azure services into an Azure VNet enables `_____` to the service from VMs or compute resources in the VNet.

%

Integrating Azure services into an Azure VNet enables **private access** to the service from VMs or compute resources in the VNet.

##

To integrate Azure services in your virtual network, you can

%

- Deploy dedicated instances of the service into a VNet
- USe Private Link
- Use Service Endpoints