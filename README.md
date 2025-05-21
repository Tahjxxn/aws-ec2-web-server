# AWS EC2 Web Server Project

This is a beginner-level project where I deployed a public-facing Apache web server using Amazon EC2 under the AWS Free Tier.

technolgies used
-Amazon EC2
-Amazon Linux 2 
-Apache HTTP Server 
-SSH 

what I did?
1. launched a t2.micro EC2 instance using the Amazon Linux 2 AMI. 
2. Opened port 80 (HTTP) and port 22 (SSH) in the security group.
3. SSH’d into the instance and installed Apache:
***bash
   sudo yum update -y
   sudo yum install httpd -y
   sudo systemctl start httpd
   sudo systemctl enable httpd 
***
4.Customized the homepage at /var/www/html/index.html.
5.Viewed the running web server in a browser using the EC2 public IP.


what i learned? 
basics of ec2 and ssh key pairs 
managing inbound security rules 
installing and managing services on Linux
responsible use of AWS resources (stop/terminate to avoid charges)

remember to stop or terminate the ec2 instance to stay within the free tier. 


May 21, 2025 
