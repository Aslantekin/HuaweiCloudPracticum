# HuaweiCloudPracticum
Project assignment of the practicum organized by Huawei Cloud and Patika.Dev.

Application Setup Steps:
All apps are built under the same VPC and Subnet.
RDS and ECS (Ubuntu 20.04) installed and EIP connected.
Two security groups were created for RDS and ECS. To ensure the security of RDS, connections to the outside world are set to only respond to requests from ECS (source security group ECS's group is selected). ECS' security group was everywhere.
Remotely connected to ECS. System updates were made and necessary frameworks were installed.
Required files from Github repo pulled to ECS.
A database was created with user name, DB name, password information in RDS and this information was entered into the python file on ECS.
Connected to MySQL from within ECS
The Python application was run and the application was accessed via the EIP address of the ECS.