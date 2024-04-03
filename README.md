# AWS_Final_Task
## Step 1: Log in into the newly created S3admin IAM user. Following the least privilege best practice this user will only have S3FullAccess policy attached to it since it aligns with the purpose and scope of the user’s task
## Step 2: We proceed to create an S3 bucket resource following the best practices and necessary configuration like allowing public access to the bucket.
## Step 3: Then we access the recently created S3 bucket properties in which we will enable the Static website hosting property specifying both index and error.html file names.
## Step 4: Then we proceed to the creation of a simple static website. For this I used a simple index.html file that I was given by Amazon Labs and added an error.html and a styles.css. Then I initialized a Git repository from my local machine using git init command and then I pushed all the changes to the repository.
## Step 5: We must prepare the GitHub Actions environment to be able to run and deploy our code to S3. The first step is to create Accees_Key and Secret_Access_Key for our S3admin user. Then we must code our deployment job in the GitHub Actions syntax.
## Step 6: The next step is to create the GitHub Actions secrets with both access keys and set them as repository secrets or environment secrets for this educational purpose. I’ve chosen repository secrets since it offers more simplicity. 
## Step 7 From the code editor terminal, I committed the changes done to my deploy.yml file which triggers the GitHub actions.
## Step 8 After the job was triggrered we proceed to check our previously empty S3 bucket with named: epamfinaltaskjoseph and it should be filled with the files that compose our simple website.
## Step 9 At this point the website won’t be reachable since the bucket is lacking the proper policies to make it available to the internet thus the next step is to add the corresponding bucket policy.
## Step 10 Now the simple static website is reachable from anywhere on the internet using the URL provided by the Simple Website Hosting service http://epamfinaltaskjoseph.s3-website-us-east-1.amazonaws.com/.
