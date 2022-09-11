S3 Versioning is very useful tool to recover from accidental overwrite and deletion of files stored in the S3 bucket.

# Step 1 - Create S3 bucket

![Screenshot (97)](https://user-images.githubusercontent.com/63674820/189517848-3e77fb17-d33a-42f8-9999-ecb7b0caad86.png)

# Step 2 - Enable bucket versioning

![Screenshot (98)](https://user-images.githubusercontent.com/63674820/189517863-28a0cd2f-689a-44a8-b52d-d4b59538f278.png)

# Step 3 - Succesful creation of bucket

![Screenshot (99)](https://user-images.githubusercontent.com/63674820/189518055-d69f4990-c2f2-4219-a461-cb2ce367a014.png)

# Now, lets upload a file to the S3 bucket and overwrite it by uploading another file with the same name

# Uploading the file

![Screenshot (100)](https://user-images.githubusercontent.com/63674820/189518108-6ba8e982-d35f-4d81-8612-777b1518e48a.png)

![Screenshot (101)](https://user-images.githubusercontent.com/63674820/189518115-2fa638ac-81eb-4f68-8a40-b4cb29c37cb5.png)

![Screenshot (102)](https://user-images.githubusercontent.com/63674820/189518123-b08e9dea-bff9-43d0-a36f-99aa06e5233a.png)

# Overwritting the file

![Screenshot (101)](https://user-images.githubusercontent.com/63674820/189518138-93828dc8-fad2-4f60-abd6-20af292ffef3.png)

# Now, using versioning to retrieve older versions

Turn on the 'Show version' button

![Screenshot (108)](https://user-images.githubusercontent.com/63674820/189518156-9ff628e0-fcbf-4974-aea2-3920582b0f3b.png)

This will show you the previous version of the file that was overwritten and the new version

If you will like to restore the previous version, first, click it --> download --> re-upload it

# Now, using versioning to retrieve deleted files

# Step 1 - Delete the file

![Screenshot (110)](https://user-images.githubusercontent.com/63674820/189519004-ce7434ea-63f5-4937-b446-3459a4c5db69.png)

File has been successfully deleted from the bucket

![Screenshot (111)](https://user-images.githubusercontent.com/63674820/189518700-e4ee23da-c31d-4406-beab-610d04df37e5.png)

# Step 2 - Show versions

The deleted file has the 'Delete marker' on it

![Screenshot (112)](https://user-images.githubusercontent.com/63674820/189518708-512790bb-b1eb-466e-bf8c-4cf3de7e5cf0.png)

# Step 3 - Delete the 'Delete marker' file to restore the file
To restore the 'delete marker' file, click the file --> delete

![Screenshot (113)](https://user-images.githubusercontent.com/63674820/189518795-5cc45406-61da-43de-89ad-51be6848a553.png)

NB: It might be a little confusing that you have to delete the delete marker file to restore the file, but thats just how it works

# Step 4 - File is restored back to the bucket

![Screenshot (115)](https://user-images.githubusercontent.com/63674820/189518827-1a563aec-f94d-4541-a0ee-a72e656c9d7a.png)
