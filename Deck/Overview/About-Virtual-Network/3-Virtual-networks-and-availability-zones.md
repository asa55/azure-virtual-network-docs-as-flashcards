###### Do VNets and subnets span all availability zones in a region?

%

Yes

###### Do you need to divide VNets and subnets by availability zones to accommodate zonal resources? Provide an example.

%

No.

For example, if you configure a zonal VM, you don't have to take into consideration the virtual network when selecting the availability zone for the VM. The same is true for other zonal resources.
