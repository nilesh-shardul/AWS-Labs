<H2> LAB DETAILS </h2>

This lab walks you through how to create a VPC using an AWS CloudFormation Stack. In this lab, we will launch an AWS CloudFormation template to create a two subnets initially. Later we update to four-subnet Amazon VPC that spans two Availability Zones.




<h2> INTRODUCTION </h2>

<H3> What is VPC? </H3>

<ol>
 <li> A VPC is similar to a computer network that we can create in an on-premises data center. In the same way, as we create dedicated and private networks within an organization, where computers in a network share network devices such as routers, switches, and so on, we can create a VPC when we create a new account in AWS.</li>

 <li> VPC makes it possible to shape similar network infrastructure as we can shape it in our own data center. The difference is, it is a virtual environment within a public cloud wherein the virtual network is logically isolated from other similar networks within the public cloud.</li>

 <li> <b> Subnet:</b> Subnet is short for the subnetwork. As we saw at the beginning of this chapter, a network is subdivided into multiple logical parts for controlling access to individual logical subparts of the network.</li>
</ol>



<H3> AWS CloudFormation </H3>

<ol>
  
 <li> CloudFormation is a service provided by AWS for designing our own infrastructure using code, i.e. infrastructure as code. </li>
  
 <li> Currently, CloudFormation supports two languages, JSON and YAML. You can write your code with one of the languages. </li>
  
 <li> CloudFormation comes with great features, being able to update your infrastructure whenever you want and also having the ability to delete the stack in case you don’t need it. </li>
  
 <li> A fascinating feature of CloudFormation is that it saves more time in building infrastructure and helps in focusing on the development. </li>
  
 <li> It is also possible to replicate our infrastructure in a short amount of time. </li>
  
 <li> It eliminates human error and works according to the code you have written. It consists of two main components, Stack and Templates. </li>

</ol>

<H3> I. CloudFormation Template </H3>

<ol>
  <li>   It consists of various sections like -
     <ul>
           <li>     AWS Template Format Version </li>            
           <li>     Description </li>            
           <li>     Metadata </li>            
           <li>     Parameters </li>            
           <li>     Mappings </li>            
           <li>     Conditions </li>            
           <li>     Resources (Required Field) </li>            
           <li>     Outputs </li>
      </ul>
  </li>
    
  <li>  It is <B>not mandatory</B> that the template requires all the above-mentioned sections. By using only the Resources section, we will be able to create a template.    </li>
    
  <li> The resources section plays an important role in the template creation. </li>
    
  <li> For example, to create an EC2 instance, a template shall consist of various parameters such as key name, image ID, instance type. </li>
    
  <li>  It is also possible to create two resources in the same template and refer to one from another, i.e. attaching an elastic IP with an EC2 instance. </li>

</ol>



<H3> II. CloudFormation Stack </H3>

<ol>
 <li> A stack consists of a collection of resources. </li>

 <li> In other words, the stack consists of one or more templates. </li>

 <li> The advantage of the stack is that it is easy to create, delete or update the collection of resources. </li>

 <li> The advanced stacks have a nested stack which holds a collection of stacks. </li>
</ol>
<H2> ARCHITECTURE DIAGRAM </h2>

![Architecture diagram1-VPC stack creation](https://github.com/nilesh-shardul/AWS-Labs/assets/40804989/6fcafa83-c3b4-425f-9e86-42f22f4dc635)

![Architecture diagram2-VPC updated stack creation](https://github.com/nilesh-shardul/AWS-Labs/assets/40804989/858bdcad-a43c-4953-9eeb-396a31d64469)

<h2> TASK DETAILS </h2>

<ol>

<li> Sign in to AWS Management Console. </li>

<li> Create Subnets using the VPC_Template cloud formation stack </li>

<li> Create Subnets using the VPC_II_Template cloud formation stack </li>

<li> Deep dive into the  VPC_Template and VPC_II_Template </li>
  
</ol>
