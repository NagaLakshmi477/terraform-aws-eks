# terraform-aws-eks

AWS account --> VPC ---> we have public subnet 

eks is in public or private subent ? --> private beacuse the trafic will take from ingrees controller (this is in public subnet )

the tarffic will go from load blancer to nodes
we need to create sg everywhre(lb,containl plan,nodes)
using bastion host we will login to ec2 if any issues
the bastion host will be public subnet

we will create VPC and sg 

bastion needs allow 443
bastion is our work station and we are using our sg in eks and we are creating loadblancer outsdde the cluster and attached to the cluster