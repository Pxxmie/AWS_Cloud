# S3 Website - Hosting a static website

1) Within our bucket, I have uploaded a jpg file. 

    ![Untitled](images/Untitled%2021.png)

2) Now go into properties on the top tab, scroll all the way down to static website hosting and click edit as we want to enable it. Click save changes after.

    ![Untitled](images/Untitled%2022.png)

    ![Untitled](images/Untitled%2023.png)

3) Now we are going to upload a index.html file in our bucket. 

    You can create index.html file by writing the following code on a note pad then saving it as index.html. 

    ```html
    <html>
    <head>
        <title>My First Webpage!</title>
    </head>
    <body>
        <h1> Cats are cute </h1>
        <p>Hello world!  </p>
        <img src="cat.jpg" width="500/">
    </body>
    </html>
    ```

    ![Untitled](images/Untitled%2024.png)

4) Now go back into properties and scroll down to static website hosting, there is a bucket website endpoint url. Copy and paste this url. You should be able to see your cat.jpg file. 

    ![Untitled](images/Untitled%2025.png)

    ![Untitled](images/Untitled%2026.png)

    You can right click the image and open in a new tab.. then you can also change the url from cat.jpg to beach and your picture of beach should appear. 

    ![Untitled](images/Untitled%2027.png)
