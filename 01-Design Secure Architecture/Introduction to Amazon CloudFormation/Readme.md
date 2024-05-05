<H2> LAB DETAILS </h2>

This lab will cover the basics of AWS CloudFormation Stack through creating a simple LAMP Server. The motive of this lab is to explore the functionality of an S3 bucket, demonstrate the process of creating a CloudFormation stack using an S3 Object URL, and guide participants through the installation of a PHP sample application.


<h2> INTRODUCTION </h2>

<H3> LAMP Server </H3>

LAMP (Linux, Apache, MySQL, PHP/Perl/Python) is an acronym denoting one of the most common solution stacks for many of the web's most popular applications. However, LAMP now refers to a generic software stack model and its components are largely interchangeable.

<H3> AWS CloudFormation </H3>

<ol>
  
 <li> CloudFormation is a service provided by AWS for designing our own infrastructure using code, i.e. infrastructure as code. </li>
  
 <li> Currently, CloudFormation supports two languages, JSON and YAML. You can write your code with one of the languages. </li>
  
 <li> CloudFormation comes with great features, being able to update your infrastructure whenever you want and also having the ability to delete the stack in case you don’t need it. </li>
  
 <li> A fascinating feature of CloudFormation is that it saves more time in building infrastructure and helps in focusing on the development. </li>
  
 <li> It is also possible to replicate our infrastructure in a short amount of time. </li>
  
 <li> It eliminates human error and works according to the code you have written. It consists of two main components, Stack and Templates. </li>

</ol>

<H3> CloudFormation Template </H3>

  

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



<H3> CloudFormation Stack </H3>
<ol>
 <li> A stack consists of a collection of resources. </li>

 <li> In other words, the stack consists of one or more templates. </li>

 <li> The advantage of the stack is that it is easy to create, delete or update the collection of resources. </li>

 <li> The advanced stacks have a nested stack which holds a collection of stacks. </li>
</ol>
<H2> ARCHITECTURE DIAGRAM </h2>

![Architecture Diagram](https://github.com/nilesh-shardul/AWS-Labs/assets/40804989/1771c9bc-0390-4bcc-8505-96579e56eeaf)

<h2> TASK DETAILS </h2>

<ol>

<li> Sign in to AWS Management Console. </li>

<li> Exploring templates in an S3 bucket. </li>

<li> Create CloudFormation Stack. </li>

<li> Testing </li>
  
</ol>
