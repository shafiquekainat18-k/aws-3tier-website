# Highly Available 3-Tier Web App on AWS

## What I built
A web app on AWS across 2 Availability Zones: an Application Load Balancer in public subnets, EC2 servers in an Auto Scaling Group in private subnets, and an RDS MySQL database in private subnets.

## Security design
- Each tier only accepts traffic
 - Servers and database are in private subnets with no public IPs
 - Access to servers through Session Manager (no SSH, no open port 22)
 - 
 ## Tests I ran
 - Terminated a server: site stayed up, replacement launched automatically
 - Stopped nginx: load balancer marked it unhealthy and stopped routing to it

 ## What I learned
 - Through this project, I gained hands-on experience building and managing cloud infrastructure using AWS. I learned how different services work together, including EC2, VPC, RDS, and Load Balancing. I also learned how AWS helps keep applications running through automatic scaling and server recovery. 


 ## Screenshots
 - Attached files 
