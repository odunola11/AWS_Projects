AWS Identity and Access Management (IAM), is used to control who or what can access AWS services and resources.


![image](https://user-images.githubusercontent.com/63674820/189516081-157bccfe-3479-45e8-a246-e42b179d7e8c.png)

# CREATING USERS IN AWS IAM

# Step 1 - Find AWS IAM
On the AWS management console, search for 'IAM'

# Step 2 - Add a user
Click on 'Users' on the left of the panel --> click on 'Add users'
Set user details, AWS access type, set password for the console as well

![Screenshot (27)](https://user-images.githubusercontent.com/63674820/189516631-e17de86f-bdbb-4156-920c-a5b2c5e37372.png)

![Screenshot (29)](https://user-images.githubusercontent.com/63674820/189516639-bb2dab71-23a3-4d73-8463-e106e98c68bc.png)

# Step 3 - Set permissions
You can set permissions by adding the user to an existing group or copy permissions of an existing user or attach exsiting permissions

In this demo i'll be using existing policies by AWS (Administrator Access)

![Screenshot (32)](https://user-images.githubusercontent.com/63674820/189516647-0fb35083-1f08-446b-831d-2bbe1ddc06a1.png)


# NB: As security best practices only give Administrative permissions only when absolutely necessary. Users should always have basic permissions required to do their jobs/tasks.


# Step 4 - Review

![Screenshot (35)](https://user-images.githubusercontent.com/63674820/189516668-1c7c04bb-b719-4828-98dc-ded2626ce478.png)

# Step 5 - Create user

![Screenshot (36)](https://user-images.githubusercontent.com/63674820/189516788-464a5513-5d57-43af-8425-8ac449e1c0ac.png)

# Step 6 - Successful creation of a user

![Screenshot (38)](https://user-images.githubusercontent.com/63674820/189516681-57cef4f7-7a31-4915-8294-79634fced4fe.png)

# CREATING GROUPS IN AWS IAM

# Step -1 Create User Group

![Screenshot (39)](https://user-images.githubusercontent.com/63674820/189516836-6f553b5e-a81c-4f24-b71d-b360212761e9.png)


![Screenshot (40)](https://user-images.githubusercontent.com/63674820/189516724-67aede68-c48c-43a0-a55c-44a791c69905.png)

# Step 2 - Set Plociies to the user group
You can use the search to find policies you might want to attach to the group

![Screenshot (43)](https://user-images.githubusercontent.com/63674820/189516727-10cb9c86-88a2-489a-bcdc-3b1e8e633dd6.png)

Step 3 - Successful creation of group

![Screenshot (44)](https://user-images.githubusercontent.com/63674820/189516738-5a34bbd8-9a72-4a08-b37a-9c4b1138ab8e.png)
