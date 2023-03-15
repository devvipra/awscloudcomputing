# How to create s3 bucket using command line.

To create any component using command line you need Access key which can be created by creatign an IAM User.
  1. Create an IAM user
  2. Assign Policy, make sure user has permission to create S3 bucket.
  3. Once user is created, click on user and go to "security Credentials" tab.
  
  ![image](https://user-images.githubusercontent.com/124074473/225457975-680aa7b6-f544-469e-b5fa-3fe0b82169a4.png)

  4. Under Access Key section click "Create Access Key". Access key in my case is disabled as i have already created two and at max you can create two access key
  
  ![image](https://user-images.githubusercontent.com/124074473/225458135-150370b9-1e30-4ff3-9bc7-4a956cad8947.png)
  5. Copy Access key and Access Secret in some safe location, Access secret is visible only once and after that you will not be able to recover.
 
 
  Now Start Gitbash or connect to ec2 instance through AWS Command line
  Once Connected, write command  "AWS configure"
  It will ask for AWS Key provide AWS key
  Then it will ask to provide AWS secret, Provide AWS secret.
  Provide region, in my case i selected us-east-2
  Provide default format as blank and press enter
  
  ![image](https://user-images.githubusercontent.com/124074473/225459445-0222cbd8-3b9f-48ea-b463-662204be9bcb.png)

 to clear screen write command clear
 
  Command to see all listed s3 bucket
   aws s3 ls
   
   Command to create bucket
    aws s3 mb s3://<bucket name>
  
  ![image](https://user-images.githubusercontent.com/124074473/225459817-705c4c4a-a3d6-467f-838d-db9951a7e148.png)

  S3 is global, so name should be unique at global level
