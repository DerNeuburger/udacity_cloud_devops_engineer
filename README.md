# Udacity Nanodegree - Cloud Devops Engineer

This repository consists of projects which were conceptualized, implemented and submitted for the nanodegree "Cloud Devops Engineer" by the online academy Udacity. Most files in this repository were created in the repository [aws_sandbox](https://github.com/DerNeuburger/aws_sandbox) which also contain the development history, because this repository only contains the files in the requested manner for submission at Udacity.

## Project 1 - Hosting Static Website using AWS S3 and Cloudfront

In this project a static website was hosted on Amazon Web Services using an Amazon S3 bucket. For better availability and improved latency, Amazon CloudFront was then added as a service to provide lower latency when requesting the website by hosting the website content additionally in Amazon's 'edge data centers' close to the actual user.

## Project 2 - Hosting a high available Web App using AWS CloudFormation

This project was dedicated to build a cloud architecture using AWS CloudFormation. AWS EC2 server instances are created in using EC2 Auto-Scaling. The source code of the web application is taken from an AWS S3 bucket hosted by Udacity. User requests to the web application are forwarded using an Application Load Balancer. The load balancer is located in a public subnet and is permitted to forward the traffic via NAT gateway to a private subnet where the web server resides. In order to allow maintenance bastion hosts are generated in the public subnets which allow inbound SSH traffic from a specific developer IP address and have the permission to SSH into the web servers. 
