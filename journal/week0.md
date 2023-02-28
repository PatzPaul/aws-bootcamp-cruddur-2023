# Week 0 — Billing and Architecture
This week starts off slow with a delay due to the AWS account set up issue but steady work continues as the issue was long resolved
I had to follow some steps from the AWS documentation to troubleshoot the issue

##Activating IAM user and role access to the Billing and Cost Management console
1.Signed in to the AWS Management Console with my root user credentials.
2.On the navigation bar, chose your account name, and then chose Account.
3.Next to IAM User and Role Access to Billing Information,I chose the Edit option.
4.Then selected the Activate IAM Access check box to activate access to the Billing and Cost Management console pages.
5.Choose Update option to now use IAM policies to control which pages a user can access.
6.After having activated IAM user access, you attached IAM policies to grant or deny access to specific billing features to my created user. 
```

```

## Here is a checklist of the cleared work 

### Recreated Conceptual Diagram on a Napkin. Tried to be as steady as possible with the hand drawing
#### Screenshot: 
file:////assets/week0/cruddur-conceptual.jpg


#### Recreated Logical Architectual Diagram in Lucid Charts
##### Screenshot:
file:///workspace/aws-bootcamp-cruddur-2023/journal/assets/week0/cruddur-logical.png

##### Link:
https://lucid.app/lucidchart/452e7be0-be3f-475c-854d-8f34c1af9efb/edit?viewport_loc=-71%2C-76%2C2368%2C1250%2C0_0&invitationId=inv_de0897dd-fbdf-4f31-82c4-baf11cd1e715

## Other tasks completed :-

### Created an Admin User	which was reinforced with MFA configurations.

### Used CloudShell to display root credentials and other information.

### Generated AWS Credentials	for a new user.

### Installed AWS CLI	on Gitpod along with the Gitpod- Github extension making it easy to work on our project.

### Created a Billing Alarm for the created account after enabling permissions for billing dashboard access to the user.
Though this is where the bulk of the time was spent as i was having a hard time with having to sort out affected policies that were not helping in giving access to the billing dashboard for the newly generated user to operate with.

### Created a Budget through the CLI commands, two in total and also looked into tags and cost explorer and other features on the billing dashboard.
### Tested creating an Amazon SNS topic and added a notification endpoint mine being email on the CLI with the delegated user account and requires confirmation once generated.

#Homework Challenges
