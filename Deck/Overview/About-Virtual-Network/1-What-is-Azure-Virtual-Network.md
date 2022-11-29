######

The abbreviation for Azure Virtual Network is

%

VNet

######

Azure Virtual Network the fundamental building block of

%

your private network in Azure

#####

Azure virtual network enables Azure resources to securely communicate with

%

- Each other
- The internet
- On-premises networks

######

VNets are similar to

%

a traditional network that you'd operate in your own data center

######

VNet offers additional benefits of Azure's infrastructure over a network you'd operate in your own data center such as

%

- Scale
- Availability
- Isolation

######

Key scenarios you can accomplish with a virtual network include

%

- Communication of Azure resources with the internet
- Communication between Azure resources
- Communication with on-premises resources
- Filtering network traffic
- Routing network traffic
- Integration with Azure resources

######

`_____` resources in a VNet can communicate `_____` to the internet, by default

%

**All** resources in a VNet can communicate **outbound** to the internet, by default

######

To communicate inbound from the internet to a resource in a VNet, assign

%

a public IP address or a public Load Balancer

######

To manage outbound connections from a VNet to the internet, you can use

%

a public IP address or public Load Balancer

######

Outbound connectivity to the internet when using only an internal Standard Load Balancer is not available until you define how you want outbound connections to work with:

%

- An instance-level public IP or
- a public Load Balancer

######

Azure resources can communicate securely with each other through

%

- a VNet
- a VNet service endpoint
- VNet Peering

######

You can connect your on-premises resources to a VNet with

%

- Point-to-site virtual private network (VPN)
- Site-to-site VPN
- Azure ExpressRoute

######

Connecting on-premises resources to a VNet using point-to-site VPN means

%

- Establishing a connection between a VNet and a single computer in your network
- Each computer that wants to establish connectivity with a VNet must configure its connection
- Communication between your computer and a VNet is sent through an encrypted tunnel over the internet
- Requires little or no changes to existing network
  - This makes point-to-site VPN well suited for
    - Developers
    - Getting started with Azure

######

Connecting on-premises resources to a VNet using site-to-site VPN means

%

- Establishing a connection between your on-premises VPN device and an Azure VPN Gateway deployed within a VNet
- Enables any on-premises resource that you authorize to access a VNet
- Communication between your on-premises VPN device and an Azure VPN gateway is sent through an encrypted tunnel over the internet

######

Connecting on-premises resources to a VNet using Azure ExpressRoute means

%

- Establishing a connection between your network and Azure, through an ExpressRoute partner
- Connection is private
- Traffic does not go over the internet

######

You can filter network traffic between subnets using

%

- Network security groups
- Network virtual appliances

######

Network security groups (and application security groups) can contain multiple inbound and outbound security rules that enable you to filter traffic to and from resources by

%

- source IP address
- destination IP address
- port
- protocol

######

A Network Virtual Appliance (NVA) is a VM that performs a network function, such as

%

- a firewall
- a WAN optimization
- or other network function

######

A list of available network virtual appliances that you can deploy in a virtual network can be found in

%

Azure Marketplace

######

By default, Azure routes traffic between

%

- Subnets
- Connected VNets
- Connected on-premises networks
- the internet

######

To override the default routes created by Azure, you can use

%

- Custom route tables
- Border gateway protocol (BGP) routes
  - (The BGP routes option only applies if you connect your virtual network to your on-premises network using Azure VPN Gateway or ExpressRoute)

######

Integrating Azure services into an Azure VNet enables

%

private access to the service from VMs or compute resources in the VNet

######

To integrate Azure services in your virtual network, you can

%

- Deploy dedicated instances of the service into a VNet, to privately access the service within the VNet and from on-premises networks
- Private Link can privately access a specific instance of the service from your VNet and from on-premises networks
- Service Endpoints can use public endpoints by extending a VNet to the service
