
# File-Provisinor-Using-Packer

This report will transfer the file from local to ami image. After that, we can create a machine from this image and already have that file.

## Apply the Packer script

1. First Setup the environment variables using below command. Replace the access and secret key with your own access and secret key:


         export ACCESS_KEY= "access key"

         export SECRET_KEY= "secret key"

2. Now, from the current directory run the following command to validate the script.

        packer validate  file_transfer.json    
        

3. Apply the packer script:

        packer build file_transfer.json