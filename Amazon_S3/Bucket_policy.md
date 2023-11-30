
# Bucket Policy

- Use it to grant public access to the bucket
- Force objects to be encrypted at upload
- Grant access to another account (Cross account)

**User Based Security** 

- IAM Policies- which API calls should be allowed for a specific user from IAM

**Resource-Based** 

- Bucket Policies bucket wide rules from the S3 console- allows cross account
- Object Access Control List (ACL) - finer grain (can be disabled)
- Bucket Access Control List (ACL)- less common (can be disabled)

## Creating a Bucket Policy

1) Now we are going to create a S3 bucket policy so my cat.jpg can be accessed through public URL. First, we go on the permissions tab. Scroll down to block public access settings and **edit**.

    ![Untitled](images/Untitled%2012.png)

    ![Untitled](images/Untitled%2013.png)

2) Untick and save changes. 

    ![Untitled](images/Untitled%2014.png)

3) Now Scroll down to bucket policy and click edit as we are going to create a bucket policy. Click on  policy generator on the top right hand side and it should take to another screen. The ARN is found under bucker ARN after you click on edit- copy and paste it onto here followed by **/*** after. 

    ![Untitled](images/Untitled%2015.png)

4) Click on Add statement, then click generate policy. 

    ![Untitled](images/Untitled%2016.png)

5) You then need to copy the policy on the edit bucket policy page and save the changes. 

    ![Untitled](images/Untitled%2017.png)

    ![Untitled](images/Untitled%2018.png)

6) Now that our object is public, lets test it by copying our object url and instead of access denied, you should be able to see your jpg file now. Any other object uploaded on this bucket will be publicly accessible through the object url. 

    ![Untitled](images/Untitled%2019.png)

    ![Untitled](images/Untitled%2020.png)
