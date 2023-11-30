# S3- Versioning

- You can version your files in Amazon S3
- It is enabled at the bucket level
- Same key overwrite will change the “version” 1,2,3
- It is best practice to version your buckets
- Protect against unintended deletes (ability to restore a version) 
- Easy roll back to previous version

1) Go into properties inside your bucket and click edit next to Bucket Versioning. Click enable and save changes. 

    ![Untitled](images/Untitled%2028.png)

    ![Untitled](images/Untitled%2029.png)

2) if we want to edit the html in our index.html file from “Cats are cute” to “Cats are really cute!!!” 

    ![Untitled](images/Untitled%2030.png)

    so we will edit our index.html file and upload the updated version. I have uploaded the file and its been overwritten now I will copy and paste the website url into the browser to see the changes. 

    ![Untitled](images/Untitled%2031.png)

    ![Untitled](images/Untitled%2032.png)

3) Go back into your bucket and click on show version toggle button.   We can see the beach.jpg and cat.jpg both have null ID as this was uploaded before we enabled versioning. However, the html has two versions, one as null which was before enabling versioning and the html file we made changes to and uploaded recently has a version ID. 

    ![Untitled](images/Untitled%2033.png)

4) However, if you want to roll back to your previous version of your html file, you can do so by clicking on the new html file we uploaded and deleting it. 

    ![Untitled](images/Untitled%2034.png)

    Now we are at the previous state of our bucket.

    ![Untitled](images/Untitled%2035.png)

    If we refresh our webpage, we should see our old version of html again. 

    ![Untitled](images/Untitled%2036.png)