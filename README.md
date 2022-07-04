<h1>Creating Static Website</h1>

<h2>Description</h2>
Amazon Simple Storage Service (Amazon S3) is an object storage service that offers industry-leading scalability, data availability, security, and performance.

This project shows how I created a static website using S3 bucket. 
<br />


<h2>Services Used</h2>

- <b>S3</b> 

<h2>Environments Used </h2>

- <b>AWS</b>

<h2>Program walk-through:</h2>
<H3>Step 1 - Creating S3 bucket</H3>

Once I had logged into the AWS account I clicked on services>S3>clicked on create bucket. I made sure the bucket name is unique or else I would not be able to create the bucket successfully. 
<img src="https://i.imgur.com/O3PUwO6.png" height="80%" width="80%" alt="Image 1"/>

Scroll down and untick block all public access. This is a safety feature of S3, but because I am intentionally creating an S3 bucket to be used as a static website, I need to untick this box. Unticking this box means that I will be able to grant public access. It does not mean that public access is granted automatically.
<br />
<br />
<img src="https://i.imgur.com/YLFvbiO.png" height="80%" width="80%" alt="Image 2"/>
<br />
<br />

<img src="https://i.imgur.com/vn34t2z.png" height="80%" width="80%" alt="Image 3"/>
<br />
<br />

<img src="https://i.imgur.com/OlsCav4.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<H3>Step 2 – Enable static website hosting </H3>
Once I had clicked on the name of my bucket, I clicked on properties and scroll down to the bottom where it says static website hosting and click on edit. I clicked  on enable and make sure host a static website is selected.
<img src="https://i.imgur.com/D92cAzu.png" height="80%" width="80%" alt="Image 4"/>
<br />
<br />
In the index document section I made sure to have added index.html and error.html in the correct text area, click save changes.
<img src="https://i.imgur.com/agU4L6a.png" height="80%" width="80%" alt="Image 6"/>
<br />
<br />
I scrolled down to static website hosting section and make a note of my bucket URL.
<img src="https://i.imgur.com/bCb30OR.png" height="80%" width="80%" alt="Image 7"/>

The next step I uploaded some objects to the bucket I have created. 

Click on upload, click on add files and add the two html files (index.html and error.html). 
<img src="https://i.imgur.com/AQICKJI.png" height="80%" width="80%" alt="Image 8"/>

<H3>Step 3 – Grant permissions</H3>
Tn this final step I had to grant permissions to be able to read the objects. I created a bucket policy. Clicked on the permission tab scroll down to where is says bucket policy click on edit. When entering the policy details remember to update the arn so it is not the same as mine or else it would not work, click on save changes.
<img src="https://i.imgur.com/mlZjKBx.png" height="80%" width="80%" alt="Image 9"/>
Based on the policy you have created you will now see a red banner stating, “publicly accessible”, which means the bucket can be access by anyone.

<img src="https://i.imgur.com/PGbBV1i.png" height="80%" width="80%" alt="Image 10"/>

This shows that I successfully created a static website in AWS
<img src="https://i.imgur.com/c8KFtkW.png" height="80%" width="80%" alt="Image 10"/>

</p>
