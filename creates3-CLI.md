# How to create s3 bucket using command line.

To create any component using command line you need Access key which can be created by creatign an IAM User.
  1. Create an IAM user
  2. Assign Policy, make sure user has permission to create S3 bucket.
  3. Once user is created, click on user and go to "security Credentials" tab.
  4. Under Access Key section click "Create Access Key"
  5. Copy Access key and Access Secret in some safe location, Access secret is visible only once and after that you will not be able to recover.
 
  
 
  Now Start Gitbash or connect to ec2 instance through AWS Command line
  Once Connected, write command  "AWS configure"
  It will ask for AWS Key provide AWS key
  Then it will ask to provide AWS secret, Provide AWS secret.
  Provide region, in my case i selected us-east-2
