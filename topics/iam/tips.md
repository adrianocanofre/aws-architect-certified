### Tips and Tricks  

* Best Practice https://aws.amazon.com/whitepapers/  
* https://docs.aws.amazon.com/general/latest/gr/aws-sec-cred-types.html
* IAM is universal, It does not apply to regions at this time
* New User have NO permissions when first created
* New Users are assigned Access Key ID & Secret Access Keys when first created
* You cannot use the Access Key ID & Secret Access Keys to login in to the console.  
* If you lose Access Key ID & Secret Access Keys, you have to regenerate them.

### Questions about IAM  

**Always setup MFA on your root account.**
 You create and customise your own password rotation policies

**Which statement best describes IAM?**
IAM allows you to manage users, groups, roles, and their corresponding level of access to the AWS Platform.

**Which of the following is not a feature of IAM?**
IAM allows you to setup biometric authentication, so that no passwords are required.  

**To save administration headaches, Amazon recommends that you leave all security groups in web facing subnets open on port 22 to 0.0.0.0/0 CIDR. That way, you can connect wherever you are in the world.**

**FALSE** is not security.  

Power User Access allows **Access to all AWS services except the management of groups and users within IAM.**  

A Policy is a document that provides a formal statement of one or more permissions.

Using SAML (Security Assertion Markup Language 2.0), you can give your federated users single sign-on (SSO) access to the AWS Management Console.


[NEXT - S3 Overview](../s3/s3.md)  
