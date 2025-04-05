#### Q9.    

![image](https://github.com/user-attachments/assets/cffe7c9c-b381-411d-9d4b-04ff4f09ae88)


#### Q10.

![image](https://github.com/user-attachments/assets/e683fe39-8dad-448c-a17a-fa17d45ddc3d)



#### Q11.

**1. Create VPC:**

• Create VPC-A and VPC-B

• VPC-A having a PUBLIC and a PRIVATE subnet.

• VPC-B contain 4 subnets (public)

**• CIDR:**

➢ VPC-A → 192.168.1.0/24

➢ VPC-B → 172.100.10.0/24

• Public Subnets are residing in AZ-ap-south-1a for VPC-A

• Private Subnets are residing in AZ-ap-south-1b for VPC-A

• Subnets of VPC-B --> 2 subnets in AZ-ap-south-1a and Another 2 subnets in AZ-ap-south-1b

**2. Create VPC-Peering:**

• Between VPC-A to VPC-B

(Create Route Tables and connect all subnets to each other)

**3. Create an EC2 Instance in default VPC (public)**

• Configure web server in ec2 instance

• Create snapshot from ec2 instance

• Create an AMI from this snapshot.

• Create Launch Template using custom AMI for VPC-B (Name→app-server)


#### Q12.


**1. Create VPC:**

Create VPC-A, VPC-B and VPC-C

Each VPC having a PUBLIC and a PRIVATE subnet.

• CIDR:

VPC-A 192.168.1.0/24

VPC-B

➤ VPC-C

192.168.2.0/24

192.168.5.0/24

Public Subnets are residing in AZ-1

Private Subnets are residing in AZ-2

**2. Create VPC-Peering:**

Between VPC-A to VPC-B

· Between VPC-B to VPC-C

Between VPC-C to VPC-A

(Create Route Tables and connect all subnets to each other)

**3. Create EC2 Instances:**

• Create one EC2 instances in each subnet.

⚫using RHEL-9 AMI.

• Configure web Server.
