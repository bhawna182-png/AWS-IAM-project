# AWS-IAM-project
IAM-access-project

What is an IAM Role
An IAM group is an identity that identifies a grouping of IAM users. You cannot sign in using a group. You may use groups to provide permissions for numerous users at once. Groups make managing permissions for big groups of users easier. 

What is an IAM service in AWS?
IAM identities can be created by the AWS account root user or an administrative user for the account. An IAM identity gives you access to your AWS account.
An IAM user group is a group of IAM users that are handled as a unit. An IAM identity is a human user or programmable workload that can be verified and then authorized to conduct operations in AWS.
Every IAM identity can be linked to one or more policies. Policies specify the activities a user, role, or member of a user group may do, on which AWS resources, as well as under what conditions.
By default, some password policies are set already , to achieve more complexity on passwords, we can change the password policy .
<img width="940" height="346" alt="image" src="https://github.com/user-attachments/assets/33c64222-d3b6-4176-bfc2-269cc2dbe3bd" />






 
At this step, we have successfully set a password policy to achieve more complexity of passwords to user. 
<img width="940" height="362" alt="image" src="https://github.com/user-attachments/assets/191159b4-3a41-42b8-b686-3a21a5b7edaf" />




Create an IAM user on our root account.
<img width="940" height="407" alt="image" src="https://github.com/user-attachments/assets/89f746d5-28fe-46a5-a1e3-e3e8c57d768a" />


 






login the AWS console via IAM user.
<img width="940" height="653" alt="image" src="https://github.com/user-attachments/assets/fad01ff8-b875-41f1-87f4-9557909b84f1" />

 



Add IAM users to a group and assign S3 read only access policy on the group which is assigned to the particular user.
<img width="940" height="297" alt="image" src="https://github.com/user-attachments/assets/c6ecf409-a723-4c30-b02b-a10f575a8098" />
<img width="940" height="410" alt="image" src="https://github.com/user-attachments/assets/64a2a228-5fec-4ef6-a4ac-051890d36ed0" />
<img width="940" height="261" alt="image" src="https://github.com/user-attachments/assets/07d89488-c559-4773-9d19-b0e73c327788" />




 
 
 



Login to AWS console as IAM user and try to create and delete object in S3 bucket created by root user but failed to perform these task because we have attached only AmazonS3ReadOnlyAcsess to this user. By this policy, the user is authorized to see the bucket and its files, but he is not authorized to delete or modify the bucket and its file.

 <img width="940" height="208" alt="image" src="https://github.com/user-attachments/assets/4e752e07-75cf-44d9-b446-6307013302c2" />
<img width="940" height="208" alt="image" src="https://github.com/user-attachments/assets/43977325-2461-4924-867a-e8b2d2db86c5" />


 


Create a role in AWS IAM to define permissions for users or services to access AWS resources. This is done to ensure that only authorized entities have the correct access levels, enhancing security and managing permissions efficiently.

<img width="940" height="470" alt="image" src="https://github.com/user-attachments/assets/877d1e80-0222-4cb3-872f-3070a01b48dd" />
<img width="940" height="606" alt="image" src="https://github.com/user-attachments/assets/22761b6f-1459-450b-a3df-c14276dca798" />
<img width="940" height="606" alt="image" src="https://github.com/user-attachments/assets/1a42d4f8-30bc-469d-97ca-ec4f92a75724" />
<img width="940" height="375" alt="image" src="https://github.com/user-attachments/assets/a230d618-c2ab-4bfd-ab1e-29152b09089d" />






 

 


 










