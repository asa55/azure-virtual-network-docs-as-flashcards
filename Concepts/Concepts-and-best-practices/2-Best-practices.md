##

As you build your network in Azure, it is important to keep in mind the following universal design principles:

%

- Ensure non-overlapping address spaces
  - Make sure your VNet address space (CIDR block) does not overlap with your organization's other network ranges
- Your subnets should not cover the entire address space of the VNet
  - Plan ahead and reserve some address space for the future
- It is recommended you have fewer large VNets rather than multiple small VNets
  - This will prevent management overhead
- Secure your VNets by assigning Network Security Groups (NSGs) to the subnets beneath them
