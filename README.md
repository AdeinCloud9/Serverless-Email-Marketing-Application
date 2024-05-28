# Serverless-Email-Marketing-Application


## Objective
Build a serverless email marketing application using AWS services, which will send emails on a schedule using HTML templates and a list of contacts stored in S3.



### Skills Learned

- Creating and managing S3 buckets. 
- Configured SES with verified email addresses and domains. 
- Creating Lambda functions using the AWS Management Console. Writing Python code for Lambda functions. Setting up and managing Lambda execution roles and permissions.
Testing Lambda functions and handling errors.
- Creating and managing IAM roles and policies. Assigning permissions to Lambda functions using IAM roles.
- Creating rules to trigger Lambda functions on a schedule. Testing and managing EventBridge rules. Understanding event-driven architectures.

### Tools Used

AWS Services Used:

AWS Simple Email Service (SES) | EventBridge | S3 | AWS Lambda | Identity & Access Management (IAM)

## Steps

*Ref 1: Web Application Architecture*
![Screenshot 2024-05-28 174236](https://github.com/AdeinCloud9/Serverless-Email-Marketing-Application/assets/170884766/309e8d2a-2fce-4f7c-8696-50b16eae06fa)

### 1. Created S3 Bucket
- Created an S3 bucket named `denttree-email-marketing`.
- Upload `email_template.html` and `contacts.csv` to the bucket.
  
  *Ref 2: S3 bucket, email_template and contacts.csv*
<img width="959" alt="Screenshot 2024-05-28 154225" src="https://github.com/AdeinCloud9/End-to-End-AWS-Web-Application/assets/170884766/3271d0dc-5959-44a5-b63c-8563aae82558">

 ![Screenshot 2024-05-28 171024](https://github.com/AdeinCloud9/Serverless-Email-Marketing-Application/assets/170884766/af8b7b45-0761-4e85-92c5-9a2281bb1794)

![Screenshot 2024-05-28 171150](https://github.com/AdeinCloud9/Serverless-Email-Marketing-Application/assets/170884766/0970a0db-d4db-49ac-8e30-996f7ab8d1bf)

### 2. Set Up SES
*Ref 3: Verified email addresses and domain in SES*
![Screenshot 2024-05-28 171332](https://github.com/AdeinCloud9/Serverless-Email-Marketing-Application/assets/170884766/620a2bb0-14fe-4228-b08b-d1d2fc4c4e95)

### 3. Created Lambda Function
- Created a Python Lambda function.
- Updated the function code with the logic to send emails.
- Assigned an execution role with permissions for S3 and SES.
  
*Ref 4: Lambda Functions*
![Screenshot 2024-05-28 171547](https://github.com/AdeinCloud9/Serverless-Email-Marketing-Application/assets/170884766/b528dc87-dff6-4d2a-be14-8f628cf9604c)

![Screenshot 2024-05-28 171702](https://github.com/AdeinCloud9/Serverless-Email-Marketing-Application/assets/170884766/513c7e93-b161-4f3e-b2f1-6f71200ce909)

### 4. Set Up EventBridge
- Created a rule in EventBridge to trigger the Lambda function on a schedule.
  
*Ref 5: Enabled schedule*
![Screenshot 2024-05-28 172009](https://github.com/AdeinCloud9/Serverless-Email-Marketing-Application/assets/170884766/0ad4e575-be95-4838-bdc2-4c14bc319ed6)


### 5. Tested the Application
- Triggered the EventBridge rule and verified emails are sent.
  
*Ref 6: Received an email*
![Screenshot 2024-05-28 172516](https://github.com/AdeinCloud9/Serverless-Email-Marketing-Application/assets/170884766/a30004fc-a088-4c05-a9e5-a7b4d6f59387)
