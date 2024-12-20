<H2> LAB DETAILS </h2>
This lab walks you through the steps to create an Application Load Balancer from AWS CLI.You will practice using AWS EC2 and AWS Load Balancers.


<h2> INTRODUCTION </h2>

<H3> AWS Elastic Load Balancer </H3>

<ol>
 <li> 	Elastic Load Balancer is used to manage load balancing between multiple EC2 instances across in multiple availability zones on AWS.</li>
 <li> 	It distributes the load across specified targets.</li>
 <li> 	It enables us to have increased availability of the application in multiple availability zones.</li>
 <li> 	It’s a fully managed service that can distribute incoming traffic to AWS resources in different availability zones.</li>
 <li> 	It monitors the health of the targets and routes traffic accordingly to the healthy targets.</li>
 <li> 	The load balancer can accept incoming traffic by configuring listeners with a protocol and port number.</li>
 <li> 	The target group can be configured with a protocol and port number to route the traffic to that particular target only if the target's health is healthy.</li>
 <li> 	Elastic load balancer supports scaling, which can be done automatically as the traffic to the application changes.</li>
 <li> 	Modification of targets from the load balancer can be done without disturbing the other requests at any point in time.</li>
</ol>

<H3> Types of Load Balancers </H3>

<H4> AWS Elastic Load balancers support 3 types of load balancing, namely: </H4>
<ol>
 <li>	Classic Load Balancer: Routing and load balancing decisions are taken at the transport layer or the application layer. It supports EC2-classic and VPC. </li>
 <li>	Network Load Balancer: Routing and load balancing decisions is taken at the transport layer. It's used for applications that need high availability and performance. </li>
 <li>	Application Load Balancer: Routing and load balancing decisions is taken at the application layer.</li>
</ol>

<H3> Application Load Balancer </H3>

<ol>
  
 <li>	Application Load Balancer is used for applications that need advanced functionality and application-level support. </li>
 <li>	It works at the application layer which is layer 7 in the OSI model. </li>
 <li>	It supports protocols such as HTTP and HTTPS only. </li>
 <li>	The application load balancer has target groups that will have registered targets such as EC2 instances. </li>
 <li>	The application load balancer routes the traffic to the specific target based on rules, even though the contents of the target instances are different. </li>
 <li>	The application load balancer acts as a one-point contact, which manages the incoming traffic. </li>
 <li>	The connection requests to the instances are managed by the load balancer with the help of listeners. </li>
 <li>	The listeners are configured with protocol and port numbers and the listeners are also configured with rules to route the traffic to the registered targets. </li>
 <li>	The listener should have a default rule so that the incoming requests are routed there by default. Other rules can be configured with suitable actions for the conditions and priority. </li>
 <li>	When the incoming request matches the condition set in the listener rule, the load balancer routes the request to that particular target group. </li>
 <li>	The target group routes the request to the registered target’s EC2 instance using the protocol and port number. </li>
 <li>	A target can be registered with multiple target groups and health check configurations can be done separately. </li>


</ol>


<H2> ARCHITECTURE DIAGRAM </h2>



<h2> TASK DETAILS </h2>

<ol>
<li>	Sign into AWS Management Console. </li>
<li>	Creating an EC2 Instance. </li>
<li>	Creating another EC2 Instance. </li>
<li>	Creating an Application Load Balancer in AWS CLI. </li>
<li>	Creating a Load Balancer. </li>
<li>	Creating 2 Target Groups. </li>
<li>	Register the Targets with their Respective Target groups. </li>
<li>	Creating Listener Default Rules. </li>
<li>	Creating Listeners for other rules. </li>
<li>	Verifying the health of the Target Groups. </li>
<li>	Verifying the Load balancer rules by accessing the DNS. </li>
<li>	Deleting AWS Resources. </li>
</ol>

  



