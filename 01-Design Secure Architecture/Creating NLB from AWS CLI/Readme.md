<H2> LAB DETAILS </h2>
This lab walks you through the steps to create and configure a network load balancer.


<h2> INTRODUCTION </h2>

<H3> AWS Elastic Load Balancer </H3>

<ol>
 <li> 	Elastic Load Balancing is one of the services provided by AWS to distribute the incoming application or network traffic across multiple targets, such as EC2 instances, containers, and IP addresses.</li>
 <li> 	ELB scales your load balancer based on traffic over time.</li>
 <li> 	ELB makes your applications highly available and fault-tolerant.</li>
 <li> 	It uses health checks to detect which instances are healthy and directs traffic only across those instances.</li>
 <li> 	You can add and remove resources from your load balancer depending on your need without disrupting the flow of requests to your applications.</li>
</ol>

<H3> Types of Load Balancers </H3>

<H4> AWS Elastic Load balancers support 3 types of load balancing, namely: </H4>
<ol>
 <li>	Classic Load Balancer - provides basic load balancing across multiple Amazon EC2 instances </li>
 <li>	Network Load Balancer - used to distribute the traffic or load using TCP/UDP protocols </li>
 <li>	Application Load Balancer - provides basic load balancing across multiple Amazon EC2 instances. </li>
</ol>

<H3> Application Load Balancer </H3>

<ol>
  
 <li>	The network load balancer (NLB) distributes the traffic based on network variables, such as IP address and destination ports. </li>
 <li>	NLB is capable of processing traffic and scaling at a much higher rate than the application load balancer. </li>
 <li>	We can't use some features of the Application Load Balancer such as SSL-offloading, host-based routing, cross-zone load balancing, and a few others. </li>
 <li>	The complete comparison among load balancers can be found in the link Load balancer differences. </li>
 <li>	It is not designed to take into consideration anything at the application layer, such as content type, cookie data, custom headers, user location, or the application behavior. </li>
 <li>	For TCP traffic, NLB selects a target using a flow hash algorithm based on the type of protocol, source IP address, source port, destination IP address and destination port. </li>
 <li>	TCP connections from a client have different source ports and sequence numbers compared with NLB and can be routed to different targets.  </li>
 <li>	Each individual TCP connection is routed to a single target for a connection. </li>
 <li>	A UDP flow has the same source and destination, so it is consistently routed to a single target throughout its lifetime.  </li>
 <li>	Different UDP flows have different source IP addresses and ports, so they can be routed to different targets.</li>
 <li>	The advantage of NLB is that it can manage the traffic to a different port to the same instance. </li>
 <li>	We can split the request based on the port to different services using the Network Load Balancer, thus NLB allows you to route the traffic among multiple applications running on the same server. </li>


</ol>


<H2> ARCHITECTURE DIAGRAM </h2>


![Architecture diagram](https://github.com/user-attachments/assets/80418f37-1978-4a46-93c7-a8d28d4187d3)


<h2> TASK DETAILS </h2>

<ol>
<li>	Sign into AWS Management Console. </li>
<li>	Creating an EC2 Instance. </li>
<li>	Creating a Network Load balancer with two target groups named apache-tg and nginx-tg. </li>
<li>	Route traffic to port 80. </li>
<li>	Attach the instance with nginx-tg to listen to the Nginx service on port 8080. </li>
<li>	Installing Apache and Nginx services in the EC2 instance. </li>
<li>	Testing the Network Load Balancer. </li>
<li>	Deleting AWS Resources. </li>
</ol>

  



