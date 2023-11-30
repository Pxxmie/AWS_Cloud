# Snow Family

Highly-secure, portable devices to collect and process data at the edge, and migrate data into and out of AWS. 

- **Data Migration**- Snowcone, Snowball Edge, Snowmobile
- **Edge Computing** - Snowcone, Snowball Edge

### Data Migrations with AWS Snow Family

Offline devices to perform data migrations- if it takes more than a week to transfer over the network, use Snowball devices. 

This means if a client has a big amount of data they want to transfer into S3 bucket, then they will request a snowball device from AWS. AWS will send the client the device by post, then the client load the data locally and ship it back to AWS, then AWS will import/export data into the S3 bucket. 

Snowball Edge (for data transfers) - 8TB

AWS Snowcone and Snowcone SSD  - 80 TB

AWS Snowmobile (actual truck) to transfer data - <100 PB

#### What is Edge Computing?

Edge location is anywhere that doesn’t have internet. For example truck on the road, ship on the sea, mining station underground.

These locations may have 

- Limited / no internet access
- Limited / no easy access to computing power

#### Snow Family - Edge Computing

- Snowcone and Snowcone SSD (smaller
- Snowball Edge - Compute optimised
- Snowball Edge- Storage optimised

All of these storage devices can run EC2 instances and AWS Lambda functions.  

**AWS OpsHub** - is a software you install on your computer/laptop to manage your snow family device. 

1) From the AWS console after searching Snow family you can click on **Order an AWS Snow Family device**.

![Untitled](images/Untitled%2058.png)

2) Select Import into Amazon S3 and click next. 

![Untitled](images/Untitled%2059.png)

3) Here you can select different snowball devices as well as pricing. 

![Untitled](images/Untitled%2060.png)

4) You can select or load an AMI, or create your own AMI. Under S3 Buckets, you can also create S3 buckets. 

![Untitled](images/Untitled%2061.png)

5) Then going forward, you can select to enable OpsHub and enter your Address details.