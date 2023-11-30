# Replication

Replication on same region or cross region. Must enable versioning when creating buckets. 

1) Create another bucket and enable versioning. 

    ![Untitled](images/Untitled%2037.png)

    ![Untitled](images/Untitled%2038.png)

1) Now create another bucket, this will be your target bucket. We can do same region replication or to replicate to another region. Enable versioning on this bucket too. 

    ![Untitled](images/Untitled%2039.png)

3) Now we should have two buckets 

    ![Untitled](images/Untitled%2040.png)

4) On origin bucket, I will upload beach.jpg in there. 

    ![Untitled](images/Untitled%2041.png)

5) On the origin bucket, click on the management tab and scroll down to replication rules, which should show that is currently 0. Click on Create replication role. 

    ![Untitled](images/Untitled%2042.png)

6) Fill in the name and select apply to all objects in the bucket under rule scope. 

    ![Untitled](images/Untitled%2043.png)

7) Select your target bucket. 

    ![Untitled](images/Untitled%2044.png)

8) Under IAM role, we will need to create a new role and save changes. 

    ![Untitled](images/Untitled%2045.png)

    ![Untitled](images/Untitled%2046.png)

9) We should now see our replication rule 

    ![Untitled](images0/Untitled%2047.png)

10) In order to test it, I will upload a new file in my origin bucket.

    ![Untitled](images/Untitled%2048.png)

11) Now lets go into our target bucket, we should the replicated image. 

    ![Untitled](images/Untitled%2049.png)