To connect private subnet ec2 instance to the internet only to download or to get any resources from the internet, we use NAT gateway.
It only allows inbound traffic means we can get any resources from the internet but we cannot send the data out from the private subnet ec2 instance.
NAT gateway should be in public subnet. when we do ssh from public subnet to private subnet under same VPC, we can connect to private subnet from public subnet but only some linux commands can be executed. 
we can not connect to internet. 
We can only connect to the internet from private subnet when we create NAT in public subnet and associate this particular NAT gateway in private subnet route table in edit routes section. means we shouls add route of NAT gateway just like we add security group
