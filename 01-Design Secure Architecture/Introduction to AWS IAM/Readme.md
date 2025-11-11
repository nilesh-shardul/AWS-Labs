# AWS EC2 Lab Guide

## **Lab Details**

Welcome to this comprehensive lab that will guide you through the process of **launching and configuring a virtual machine** in the powerful and dynamic **Amazon Web Services (AWS)** cloud.

In this lab, you will gain practical experience using **Amazon Machine Images (AMI)** to launch **Amazon EC2 instances** and master the art of using **key pairs for SSH authentication** to log into your instance.  
Additionally, you will learn how to **create a web page and publish it** on your AWS virtual machine.

- **Duration:** 30 minutes  
- **AWS Region:** US East (N. Virginia) — `us-east-1`

---

## **Introduction**

### **What is EC2?**

**Amazon Elastic Compute Cloud (EC2)** is a cloud-based web service that provides **resizable compute capacity** in the AWS Cloud.  
It enables users to **rent virtual machines (instances)** and run applications without the need to invest in physical hardware.

Here are some **key highlights** of Amazon EC2:

- **Full Control:**  
  Customize your virtual computing environment with your choice of operating system, programming languages, and application servers.

- **Security:**  
  Configure **Security Groups** and **Network ACLs** to control inbound and outbound traffic to your instances, ensuring a secure environment.

- **Flexible Pricing Options:**  
  Choose from **On-Demand**, **Reserved**, or **Spot Instances** to optimize costs based on your workload and budget.

- **Monitoring & Logging:**  
  Use **Amazon CloudWatch** to monitor performance and **CloudTrail** to track API activity across your AWS account.

- **Storage Options:**  
  Select from **EBS**, **EFS**, or **Instance Store** volumes to match your application’s storage needs.

- **Custom AMIs:**  
  Create **Amazon Machine Images (AMIs)** from your configured instances to launch new instances with the same software stack.

> 💡 With its flexibility, scalability, and reliability, EC2 has become the **go-to compute platform** for developers, startups, and enterprises worldwide.

---

## **Architecture Diagram**

Below is the architecture representation of this lab setup:

![EC2 Architecture Diagram](image1.png)

---

## **Task Details**

You will perform the following tasks during this lab:

1. **Sign in** to the AWS Management Console  
2. **Launch an EC2 instance** with desired specifications  
3. **SSH** into the EC2 instance using the key pair  
4. **Install Apache server** on the instance  
5. **Create a web page** and host it on the EC2 instance  
6. **Validate the lab** setup and ensure the web page is accessible

---

## **Launching the Lab Environment**

To begin the lab:

1. Click the **Start Lab** button.
2. Wait until the **cloud environment is provisioned**.  
   > ⏳ This process takes **less than a minute**.
3. Once the environment starts, you will be provided with:
   - **IAM Username**
   - **Password**
   - **Access Key**
   - **Secret Access Key**

You’ll use these credentials to access and configure your AWS resources throughout this lab.

---

*End of Lab Details Section*
