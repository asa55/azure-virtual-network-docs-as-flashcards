###### Official abbreviation for Azure Virtual Network

%

VNet

###### What is Azure Virtual Network the fundamental building block of?

%

Your private network in Azure

###### What does Azure virtual network enable Azure resources to do?

%

Securely communicate with:

- Each other
- The internet
- On-premises networks

###### What traditional alternative is VNet similar to?

%

A network that you'd operate in your own data center

###### What advantages does VNet offer over a network you'd operate in your own data center?

%

VNet brings with it additional benefits of Azure's infrastructure such as:

- Scale
- Availability
- Isolation

###### What are key scenarios you can accomplish with a virtual network?

%

- Communication of Azure resources with the internet
- Communication between Azure resources
- Communication with on-premises resources
- Filtering network traffic
- Routing network traffic
- Integration with Azure resources

###### Can resources in a VNet communicate to the internet by default?

%

All resources in a VNet can communicate **outbound** to the internet, by default

###### How to communicate inbound from the internet to a resource in a VNet?

%

Assign a public IP adress or a public Load Balancer

###### How to manage outbound connections from a VNet to the internet?

%

You can use public IP or public Load Balancer to manage outbound connections

###### What condition must be met to enable outbound connectivity to the internet when using only an internal Standard Load Balancer?

%

Outbound connectivity is not available until you define how you want outbound connections to work with:

- An instance-level public IP or
- a public Load Balancer

###### List the ways in which Azure resources can communicate securely with each other

%

- Through a VNet
- Through a VNet service endpoint
- Through VNet Peering

###### List the ways in which you can connect your on-premises resources to a VNet

%

- Point-to-site virtual private network (VPN)
- Site-to-site VPN
- Azure ExpressRoute

###### List features of connecting on-premises resources to a VNet using point-to-site VPN

%

- Established between a VNet and a single computer in your network
- Each computer that wants to establish connectivity with a VNet must configure its connection
- Communication between your computer and a VNet is sent through an encrypted tunnel over the internet
- Requires little or no changes to existing network
  - This makes point-to-site VPN well suited for
    - Developers
    - Getting started with Azure

###### List features of connecting on-premises resources to a VNet using site-to-site VPN

%

- Established between your on-premises VPN device and an Azure VPN Gateway deployed within a VNet
- Enables any on-premises resource that you authorize to access a VNet
- Communication between your on-premises VPN device and an Azure VPN gateway is sent through an encrypted tunnel over the internet

###### List features of connecting on-premises resources to a VNet using Azure ExpressRoute

%

- Established between your network and Azure, through an ExpressRoute partner
- Connection is private
  - Traffic does not go over the internet

###### List the ways in which you can filter network traffic between subnets

%

- Network security groups
- Network virtual appliances

###### List features of using network security groups to filter network traffic between subnets

%

Network security groups (and application security groups) can contain multiple inbound and outbound security rules that enable you to filter traffic to and from resources by:

- source IP address
- destination IP address
- port
- protocol

###### What is a Network Virtual Appliance (NVA)?

%

A network virtual appliance is a VM that performs a network function, such as:

- a firewall
- a WAN optimization
- or other network function

###### Where can you find a list of available network virtual appliances that you can deploy in a virtual network?

%

Azure Marketplace

###### What does Azure route traffic between, by default?

%

- Between subnets
- Connected VNets
- Connected on-premises networks
- the internet

###### List your options to override the default routes created by Azure

%

- Custom route tables
- Border gateway protocol (BGP) routes
  - (The BGP routes option only applies if you connect your virtual network to your on-premises network using Azure VPN Gateway or ExpressRoute)

###### What does integrating Azure services into an Azure VNet enable?

%

Private access to the service from VMs or compute resources in the VNet

###### List the ways in which you can integrate Azure services in your virtual network

%

- Deploy dedicated instances of the service into a VNet, to privately access the service within the VNet and from on-premises networks
- Private Link can privately access a specific instance of the service from your VNet and from on-premises networks
- Service Endpoints can use public endpoints by extending a VNet to the service
