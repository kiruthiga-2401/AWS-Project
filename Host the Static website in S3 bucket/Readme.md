# How to host Static Website on Amazon S3
Amazon Simple Storage Service (Amazon S3) can be used to host static Websites without a need for a Web server (at an extremely low cost). S3 buckets can be used to host the HTML, CSS and JavaScript files for entire static websites.

Introduction A website is static when the system services used to render web pages and scripts are all client rather than server-based. On the other hand, a dynamic website relies on server-side processing, including server-side scripts such as PHP, JSP, or ASP.NET

Most websites are becoming static websites which means they run zero server side code and consist of only HTML, CSS and JavaScript. With no server side code to run, there is no reason to host them on a traditional server.

You can start by creating an Amazon S3 bucket, enabling the Amazon S3 Website hosting feature, and configuring access permissions for the bucket. After you have uploaded files and setup Website, Amazon S3 takes care of serving your content to your visitors.
You can start by creating an Amazon S3 bucket, enabling the Amazon S3 Website hosting feature, and configuring access permissions for the bucket. After you have uploaded files and setup Website, Amazon S3 takes care of serving your content to your visitors.

Amazon Route 53: You can also use Amazon Route 53 (a managed Domain Name System (DNS) service) to point your domain to your Amazon S3 bucket.

Amazon CloudFront: You can also use Amazon CloudFront to enable your website to load quickly. Amazon CloudFront will create a content delivery network (CDN) that hosts your website content in close proximity to your users.

# Advantages of Hosting Website on S3
Here are some of the advantages of hosting site on S3
Performance: The website will be highly performant and scalable at a fraction of the cost of a traditional Web server.

Scalability: Amazon S3 is inherently scalable. For popular websites, the Amazon S3 architecture will scale seamlessly to serve thousands of HTTP requests per second without any changes to the architecture.

Availability: In addition, by hosting with Amazon S3, the website is inherently highly available.

# Set-Up Instructions
### Step 1: Create a s3 Bucket when you first create an s3 bucket, you select the AWS region in which the files whill be geographically stored.
click on "create bucket" button

<img width="1366" height="768" alt="Screenshot (212)" src="https://github.com/user-attachments/assets/d3145afe-7b93-4825-be76-45ce3c5b95d5" />

### Step-2: Upload content of your website to your s3 buckets 
<br>

<img width="1366" height="632" alt="Screenshot (231)" src="https://github.com/user-attachments/assets/f27eb7c4-76d4-4434-88be-f3e92995ff63" />
<br>

### Step - 3 Edit the host static
<br>

<img width="1365" height="631" alt="Screenshot (230)" src="https://github.com/user-attachments/assets/76710ea7-551e-48b7-a7ba-6c80d0f3c2c7" />
<br>

Give the index name of the website
<br>

<img width="1365" height="552" alt="Screenshot (229)" src="https://github.com/user-attachments/assets/218891c7-7c4c-45d5-9b80-91f2da977488" />
<br>

### Step-4: Add a bucket policy to allow public read access 
Uncheck manage public bucket policies:
Uncheck- Block new public policies(recommended)
Uncheck - Block public and cross-account access if bucket has public policies
<br>

<img width="1360" height="661" alt="Screenshot (228)" src="https://github.com/user-attachments/assets/4ed3a022-373d-4a7c-b359-4e64697dab5c" />
<br>

### Step-5: Enable ACl
<br>

<img width="1366" height="685" alt="Screenshot (226)" src="https://github.com/user-attachments/assets/6355f8b3-0985-4654-a00c-7f11ffbd4452" />

<br>

### Step-6: Make a public using Acl
<br>

<img width="1366" height="685" alt="Screenshot (226)" src="https://github.com/user-attachments/assets/289cfbf3-9d8d-4653-80c7-af85597c2b72" />

<br>

### Step-7:Access your website using url
<br>

<img width="1343" height="535" alt="we" src="https://github.com/user-attachments/assets/c751a0ea-506c-4f38-9ba1-5a95d3463ad2" />








