\# AWS IAM Lab Guide



\## Lab Steps



---



\### \*\*Task 1: Sign in to the AWS Management Console\*\*



Click on the \*\*Open Console\*\* button. You will be redirected to the AWS Console in a new browser tab.



On the \*\*AWS sign-in page\*\*:



\- Leave the \*\*Account ID\*\* as default.  

&nbsp; > ⚠️ \*\*Never edit or remove\*\* the 12-digit Account ID present in the AWS Console. Otherwise, you cannot proceed with the lab.



\- Copy your \*\*Username\*\* and \*\*Password\*\* from the Lab Console to the \*\*IAM Username\*\* and \*\*Password\*\* fields in the AWS Console.



\- Click \*\*Sign In\*\*.



Once signed in to the AWS Management Console:



\- Set the default AWS Region as \*\*US East (N. Virginia)\*\* — `us-east-1`.



---



\### \*\*Task 2: Create IAM Users\*\*



In this task, we will create new IAM users by providing their name, password, permissions, and tags.  

These users will later be added to their respective groups.



1\. Click on \*\*Services\*\* and select \*\*IAM\*\* under \*\*Security, Identity, \& Compliance\*\*.

2\. In the \*\*IAM Dashboard\*\*, select \*\*Users\*\* from the left panel and click \*\*Create User\*\*.



\#### \*\*Add User Details\*\*

\- \*\*User name:\*\* `John` (or desired name)

\- Check \*\*Provide user access to the AWS Management Console - optional\*\*

\- Select \*\*Custom password\*\* and enter `whizlabs@123` (or desired password)

\- Uncheck \*\*Users must create a new password at next sign-in\*\*

\- Click \*\*Next\*\*



!\[Add IAM User](image1.png)



\#### \*\*Set Permissions\*\*

\- Keep default permissions.

\- Click \*\*Next\*\*.



\#### \*\*Add Tags\*\*

\- Click \*\*Add new tag\*\*

&nbsp; - \*\*Key:\*\* `Dev-Team`  

&nbsp; - \*\*Value:\*\* `Developers`



!\[Add Tags](image2.png)



Click \*\*Create User\*\*.



> 📝 \*\*Note:\*\* Ignore any error that appears while creating users and click \*\*Close\*\*.



Click \*\*Return to users list\*\* and then \*\*Continue\*\*.



\#### \*\*Repeat the same steps\*\* for the following users:



| User Name | Custom Password | Key      | Value      |

|------------|----------------|-----------|-------------|

| Sarah      | whizlabs@123   | Dev-Team  | Developers  |

| Ted        | whizlabs@123   | HR-Team   | HR          |

| Rita       | whizlabs@123   | HR-Team   | HR          |



✅ You have successfully created \*\*4 IAM users\*\*: John, Sarah, Ted, and Rita.



!\[IAM Users Created](image3.png)



---



\### \*\*Task 3: Create IAM Groups and Add IAM Users\*\*



In this task, we will create new IAM groups, add users to their respective groups, and attach policies to grant specific access.



1\. Select \*\*User groups\*\* from the left panel.

2\. Click \*\*Create group\*\*.



\#### \*\*Create Dev-Team Group\*\*



\- \*\*User group name:\*\* `Dev-Team`

\- Under \*\*Add Users to the group\*\*, select:

&nbsp; - John  

&nbsp; - Sarah



Scroll down to \*\*Attach permissions policies\*\*:



\- Search and select:

&nbsp; - `AmazonEC2ReadOnlyAccess`

&nbsp; - `AmazonS3ReadOnlyAccess`



> ⚠️ \*\*Note:\*\* Do not add other policies. Adding unlisted policies will cause an error.



Review details and click \*\*Create group\*\*.



!\[Dev Team Group](image4.png)



\#### \*\*Create HR-Team Group\*\*



Repeat the same steps:

\- \*\*User group name:\*\* `HR-Team`

\- Add users:

&nbsp; - Ted  

&nbsp; - Rita

\- Attach the following policy:

&nbsp; - `Billing`



> ⚠️ Do not add other policies than the ones mentioned above.



Review and click \*\*Create group\*\*.



!\[HR Team Group](image5.png)



---



\### \*\*Do You Know?\*\*



💡 \*\*AWS IAM Access Analyzer (2021)\*\* introduced automated reasoning to help identify resources that an IAM policy allows or denies access to.  

This feature is useful for:

\- Detecting unintended access

\- Auditing IAM policies for compliance

\- Getting recommendations to remove unintended access



Access Analyzer makes it easier to maintain a \*\*secure AWS environment\*\*.



---



\### \*\*Task 4: Validation Test\*\*



After completing all steps:



1\. Click the \*\*Lab Validation\*\* button on the left panel.

2\. Select \*\*Validate My Lab\*\* on the \*\*Lab Validation\*\* tab.



This will validate the AWS resources and display whether you completed the lab successfully.



\*\*Sample Output:\*\*



!\[Lab Validation Output](image6.png)



---



\## \*\*Completion and Conclusion\*\*



In this lab, you:



\- Created \*\*4 IAM users\*\* and \*\*2 IAM groups\*\*

\- Attached required \*\*IAM policies\*\*

\- Added \*\*John and Sarah\*\* to the \*\*Dev-Team\*\* group

\- Added \*\*Ted and Rita\*\* to the \*\*HR-Team\*\* group



\### ✅ You Learned:

\- How to create IAM users and groups  

\- How to add users to IAM groups  

\- How to attach policies during IAM group creation  

\- How to allow specific users or groups to access AWS services and resources



---



\*End of Lab\*



