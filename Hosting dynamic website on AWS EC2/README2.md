## Session manager can be used instead of SSH to have access to an EC2 instance; this is a more secure option

# Step 1 - Create a role for session manager

### When creating the role for EC2 to access S3, also assign a role for session manager

![Screenshot (145)](https://user-images.githubusercontent.com/63674820/189738445-71cf690f-9f4a-4106-8641-5c5ec2e306dc.png)

### Launch your EC2 instance

# Step 2 - Start session manager

### AWS management console --> AWS systems manager --> Session manager --> start session

![Screenshot (182)](https://user-images.githubusercontent.com/63674820/189739185-24f4c6a7-2c6c-4422-8acc-78441bc98e4d.png)


# Step 3 - Select target instance

![Screenshot (183)](https://user-images.githubusercontent.com/63674820/189739330-a0e2cf46-d189-4713-994e-a8626d7c3659.png)

### And there you have your terminal 

![Screenshot (184)](https://user-images.githubusercontent.com/63674820/189739386-5e1ad35a-c79b-4a14-b031-202abd0a81f3.png)
