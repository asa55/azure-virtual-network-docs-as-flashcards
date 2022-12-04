##

As you build your network in Azure, it is important to keep in mind the following universal design principles:

%

- Ensure non-overlapping address spaces
- Your subnets should not cover the entire address space of the VNet
- It is recommended you have fewer large VNets rather than multiple small VNets
- Secure your VNets by assigning Network Security Groups (NSGs) to the subnets beneath them

##

To ensure non-overlapping address spaces make sure your VNet address space (CIDR block) does not overlap with

%

your organization's other network ranges

##

To ensure your subnets do not cover the entire address space of the VNet, plan ahead and

%

reserve some address space for the future

##

It is recommended you have fewer large VNets rather than multiple small VNets because this will prevent

%

management overhead
