# Hosting a dynamic website on EC2

# Step 1 - Create an S3 bucket and upload your site configuration files

### This is to create where to store the config files for EC2 to access later to host the website


### This has already been covered in a different project; link below

https://github.com/odunola11/AWS_Projects/tree/main/Hosting%20static%20website%20on%20AWS%20S3

# Step 2 -  Create a role for EC2 to access S3

### Go to IAM --> Roles --> Create role


![Screenshot (124)](https://user-images.githubusercontent.com/63674820/189732005-629df9f9-5bd6-44aa-a0ce-847e778222b5.png)

# Step 3 - Select trusted entity type


### Since we are creating this role to give access to EC2, we'll be selecting 'AWS service'


![Screenshot (125)](https://user-images.githubusercontent.com/63674820/189732117-a95fa9d8-9af0-40fc-8445-62c5601f7b70.png)


# Step 4 - Add permissions


### Here, we'll be granting full access to S3


![Screenshot (126)](https://user-images.githubusercontent.com/63674820/189732441-50fc2baf-497f-45e5-944c-52d6ca58e238.png)


# Step 5 - Name, review and create


![Screenshot (128)](https://user-images.githubusercontent.com/63674820/189732571-e19690a2-b5a8-49c2-9d25-6ba4b053f1c8.png)


# Step 6 - Launch EC2 instance


![Screenshot (131)](https://user-images.githubusercontent.com/63674820/189732730-79486cc1-d5a5-4f6a-b05c-e62e2aded015.png)

![Screenshot (132)](https://user-images.githubusercontent.com/63674820/189732774-7963acf7-d8cc-4af4-bb48-931f5f04ea96.png)


# Step 7 - Set up Security group rules

### Here, we'll be setting 3 inbound rules, HTTP and HTTPS (for public users) and SSH (for adminstrative use)


![Screenshot (133)](https://user-images.githubusercontent.com/63674820/189733421-3f447291-5d8d-4899-8262-c78aa08e5c01.png)


## NB: the SSH source IP should be your own IP address.


# Step 8 - Set up key pair


### This is important for when you want to access the EC2 instance via SSH


![Screenshot (134)](https://user-images.githubusercontent.com/63674820/189733629-405c7ee9-436a-49e5-ad65-9666eba2049f.png)


# Step 9 - Launch instance


![Screenshot (135)](https://user-images.githubusercontent.com/63674820/189733746-492665b3-bd77-4ddf-9a7d-97c632fbb4e5.png)


# Step 10 - SSH into the instance for configuration


## Step 10.1 First, ensure the instance status says 'Running' and status check says '2/2 checks passed'


![Screenshot (136)](https://user-images.githubusercontent.com/63674820/189734106-18cabab9-0c86-45e2-8c02-4ea785235d41.png)


## Step 10.2 To SSH into the instance you can use tools like MobaXterm or PuTTY, here we'll be using PuTTY


### NB: Make sure to get your public IPv4 address from the EC2 instance


![Screenshot (140)](https://user-images.githubusercontent.com/63674820/189734726-83c9875c-ba08-45d8-83b9-906af2b9d0fd.png)


## Step 10.3 Use the PuTTY key generator to generate a key for the connection by inputting the key pair generated in step 8 above


## Step 10.4 In the PuTTY GUI, under connections --> SSh --> Auth --> Browse the location to the generate key --> open


![Screenshot (141)](https://user-images.githubusercontent.com/63674820/189735943-a1177c65-352d-477c-9fb1-e3dcd3017e48.png)


## Step 10.5  Enter the following code in the terminal download Apache and point the EC2 to the S3 bucket


![Screenshot (139)](https://user-images.githubusercontent.com/63674820/189736059-e04f56af-0bcf-440c-96d5-e4c7fe064588.png)


![Screenshot (137)](https://user-images.githubusercontent.com/63674820/189736268-823210ee-27e4-48af-a0f0-8626c948573a.png)


# Step 11 - If all went well, your dynamic site should be live


![Screenshot (138)](https://user-images.githubusercontent.com/63674820/189736681-90392e86-13bf-4eeb-b0db-01fd5439c54a.png)
