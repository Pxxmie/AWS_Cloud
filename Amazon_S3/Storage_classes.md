# Storage Classes

Can move between classes manually or using S3 lifecycle configurations

1) Create a new bucket and give it a suitable name - “s3-storage-classes-demo”

    ![Untitled](images/Untitled%2050.png)

2) Now, I want to upload an object inside my bucket. After uploading, scroll down to properties on the upload page. 

    ![Untitled](images/Untitled%2051.png)

3)  We are going to select **Standard-IA** and create an object there and press upload. 

    ![Untitled](images/Untitled%2052.png)

4) If we go into the overview of our object, we can see the storage class. However if we ever want to change it we can do so by scrolling down to storage class and clicking edit. 

    ![Untitled](images/Untitled%2053.png)

    then we can change to a different class. 

    ![Untitled](images/Untitled%2054.png)

5) Now we are going to automate how we can move these objects between different storage classes. So back to your object and click management and click on create lifecycle rule. 

    ![Untitled](images/Untitled%2055.png)

6) We want to the rule scope to **apply to all objects in the bucket** and then select rule actions to **move current versions of objects between storage classes.**

    ![Untitled](images/Untitled%2056.png)

7) Then we can automate the transitions by adding a rule here and selecting the storage classes. 

    ![Untitled](images/Untitled%2057.png)