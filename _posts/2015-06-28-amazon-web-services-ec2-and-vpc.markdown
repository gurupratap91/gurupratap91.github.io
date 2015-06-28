---
layout: post
title:  "Amazon Web Services EC2 and VPC"
date:   2015-06-28 16:15:00
categories: jekyll update
---

<html>
	<head>
		<title>Amazon Web Services: EC2 and VPC</title>
	</head>
<body>
<p>
As the wiki page says Amazon Web Services is a collection of remote computing services. It is an IaaS(Infrastructure as a Service). IaaS is a form of cloud computing that provides virtualized computing resources over the Internet. IaaS is one of three main categories of cloud computing services, alongside Software as a Service (SaaS) and Platform as a Service (PaaS). AWS has several services available to serve the requirements of it's users. I used the Amazon EC2(Elastic Cloud Computing) and Amazon VPC(Virtual Private Cloud) services.
</p>
<p>
Amazon EC2 provides elastic cloud infrastucture which solves the problem of scalability for developers. It saves both time and money as it provides a very simple interface for setting up machines and allows you to pay only for the resources that you require. It provides options from small and economical servers for small applications to cluster computing instances designed for high performance computing. It also allows to set the CPU, memory and storage needs individually to meet application specific requirements. To ensure security, instances launched are located in a VPC(Virtual Private Cloud) which is a logically isolated network. It provides auto scaling feature to increase the number of instances depending upon the load on your servers. Settings for these can be customized based on your needs.
</p>
<p>
Amazon VPC allows you to create a virtual private network that you define. It gives complete control over the instances that you would launch. You can specify the IP address range, create subnets and configure route tables and network gateways. Depending on your need you can create private(which cannot be accessed directly from the internet)or public subnets. Security can be enhanced with the use of Security Groups and Network ACLs which allow you to define security rules at instance level and subnet level respectively. Adding these allows you to list what all traffic you want to allow through you instance or subnet. It gives you complete control over your virtual networking environment.
</p>
<p>
While launching instances on the cloud you get the option to select from different AMI's(Amazon Machine Images) available to use. These AMI's have preconfigured settings e.g. free tier Amazon Linux instance will have some prior configuration put on a linux environment(For details <a href = "http://aws.amazon.com/amazon-linux-ami/">click here</a>). You can configure these systems according to your needs and even save them as AMI's for future need. This solves the problem of configuring all instances separately. Try launching an instance of your own after setting up a VPC on EC2. If you have an AWS account you can set up a micro instance for free. Documentation available for AWS is quite good and easy to follow. 
</p>

Use these links for information related <i><a href="http://aws.amazon.com/ec2/">EC2</a></i> and <i><a href="http://aws.amazon.com/vpc/">VPC</a></i>
</body>
</html>
