# Networking in the Cloud 1

## Story

You have just been given a cloud project that is going to be deployed using AWS. No further details have been provided other than it is going to require a lot of networking architechute, VPCs, private and public subnets, incoming and outgoing as well as traffic in between. You are provided with an AWS account you can explore and play with.

## What are you going to learn?

- What resources has AWS created for you
- How to create a VPC in AWS
- How to create a private subnet in AWS
- How to create a public subnet in AWS
- How to create an Internet Gateway in AWS
- How to create Route Tables in AWS

## Tasks

1. AWS has already created a few resources for you. Go ahead and explore all pre-configured resources in AWS Management Console.
    - Identify default VPC Name, VPC ID, State, CIDR blocks.
    - Identify all default subnets. How many subnets has AWS created for you? What are the IDs, VPC, and CIDR blocks?
    - Identify all route tables. What is the Route Table ID? Is it associated with a VPC? How many routes are there? Their destination, target, and status.
    - Is there an Internet Gateway, IGW? What is the ID? What is the state and where is it attached to?

2. [OPTIONAL] Create a new VPC called `my-vpc` with CIDR 10.10.0.0/16.
    - A new VPC is created

3. [OPTIONAL] Create a new subnet `my-private-subnet` in `my-vpc` VPC with CIDR 10.10.0.0/24. Create another subnet `my-public-subnet` in `my-vpc` VPC with CIDR 10.10.1.0/24.
    - A subnet called `my-private-subnet` in `my-vpc` VPC with CIDR 10.10.0.0/24 is created.
    - A subnet called `my-public-subnet` in `my-vpc` VPC with CIDR 10.10.1.0/24 is created.

4. [OPTIONAL] Create an Internet Gateway called `my-internet-gateway` and attach it to the VPC.
    - A new Internet Gateway called `my-internet-gateway` is created.
    - The Internet Gateway is attached to the VPC.

5. [OPTIONAL] Create a route table called `my-public-rt` and associate it with the public subnet. Add a route with destination 0.0.0.0/0 and target the Internet Gateway.
    - A route table is created and associated with the public subnet.
    - A route with destination 0.0.0.0/0 and target IGW is created.

## General requirements

None

## Hints

- You have a default VPC in each AWS Region. A default VPC is ready for you to use, you are strongly encouraged to play with that default VPC and then set this up yourself, because when you set it up yourself you get to choose what all the variables should be.
- Most of VPC, Subnet, Routing Table and IGW components should be self-explanatory by now, but if some are unclear or in doubt, refer to background materials and/or tutorials.

## Background materials

- <i class="far fa-exclamation"></i> [VPC Route Tables](https://docs.aws.amazon.com/vpc/latest/userguide/VPC_Route_Tables.html)
- <i class="far fa-exclamation"></i> [VPC Peering](project/curriculum/materials/pages/networks/networking-in-the-cloud.md)
- <i class="far fa-video"></i> [A Day in the Life of a Billin Packets](https://www.youtube.com/watch?v=Zd5hsL-JNY4)
- <i class="far fa-book-open"></i> [Getting started with AWS VPC](https://medium.com/better-programming/getting-started-with-aws-vpc-ae23ecf75743)
- <i class="far fa-book-open"></i> [AWS Routing 101](https://medium.com/@mda590/aws-routing-101-67879d23014d)
- <i class="far fa-video"></i> [AWS Networking Fundamentals](https://www.youtube.com/watch?v=hiKPPy584Mg)
