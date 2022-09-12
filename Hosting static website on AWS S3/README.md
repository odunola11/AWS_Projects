# S3 can be used to host a static website 

# Step 1 - Create an S3 bucket

![Screenshot (75)](https://user-images.githubusercontent.com/63674820/189721955-c1d3c42a-b4dc-40ec-8e2e-9c8333dcd62b.png)

# Step 2 - Uncheck Block all public access
We are turning this off because this site we will be creating will be a public facing one

![Screenshot (76)](https://user-images.githubusercontent.com/63674820/189722260-b75d9bb8-525b-4ac8-8067-ed4ecd29d379.png)

# Step 3 - Enable default encryption

![Screenshot (78)](https://user-images.githubusercontent.com/63674820/189722502-651a1990-c18d-4373-8237-b8e63a6ee7de.png)

# Step 4 - Create bucket

![Screenshot (81)](https://user-images.githubusercontent.com/63674820/189722681-13e3ea63-e033-4a67-9667-c3fdcedc3f69.png)

# Step 5 - Upload your website file to the S3 bucket

![Screenshot (82)](https://user-images.githubusercontent.com/63674820/189724432-82d25d79-6501-439c-bc61-075138eaac90.png)

![Screenshot (83)](https://user-images.githubusercontent.com/63674820/189724749-692db4e9-d999-409f-b531-0b1df54e4fe8.png)

# Step 6 - Set up hosting static website

After uploading the files go to the properties pane in the bucket

![Screenshot (86)](https://user-images.githubusercontent.com/63674820/189724992-824e3ae4-ea58-4b33-b037-e035daec1453.png)

Scroll down to 'Static website hosting' --> Edit

# Step 7 - Edit static website hosting

![Screenshot (88)](https://user-images.githubusercontent.com/63674820/189725230-96cb966c-81c1-49d1-b1a0-d34fca5fd3fa.png)

Point to your webisite home page, here it is index.html

![Screenshot (89)](https://user-images.githubusercontent.com/63674820/189725483-e0ce16c2-8da4-4842-ac5b-b0c8ef349be4.png)

# Step 8 - Successful hosting of static website

![Screenshot (90)](https://user-images.githubusercontent.com/63674820/189725627-a51f4a37-f149-4c63-977e-482e77da258c.png)

# Step 9 -  Set up bucket policy for public read access

![Screenshot (94)](https://user-images.githubusercontent.com/63674820/189726278-eb539597-5bac-4c55-a218-27f264071e46.png)

NB: Ensure where highlighted in red above is replaced with your own S3 arn

![Screenshot (96)](https://user-images.githubusercontent.com/63674820/189726535-8e5d7283-df5f-4c66-8da0-3b8bd293bfd4.png)

# Step 10 - Access the site

![Screenshot (91)](https://user-images.githubusercontent.com/63674820/189726942-8dbcc673-9de8-40e4-a29d-7304909b8a55.png)

