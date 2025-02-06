Chaitanya Chaudhari
cchaudha@gmu.edu
SWE 642 Assignment 1

This assignment contains:

A index.html page - Has my personal Introduction page with a picture and brief description about myself. A student class Webpage. It contains links to CS Department Information page and Student Survey Form . You can find the button link on top at the header section of this page.

A department.html - A CS Department Information page. With two paragraphs, a MS degrees List and the required courses as per each degree table. It also links to the student survey form page. You can find the button link on top at the header section of this page.

A survey.html - It has a student survey form made keeping in mind all the requirements mentioned on the assignemnt question. Facility has been given to navigate from any of the 3 pages to the others.

An images folder - which contains images  used for this assignment.

bootstrap.min.css and bootstrap.min.js files

A readme.md file

Styling sheets(department.css, style.css and survey.css) for all the 3 pages 

Part 1 :

Please check out my assignment below hosted on AWS S3 bucket:
http://cchaudha-swe642-hw1-bucket.s3-website-us-east-1.amazonaws.com

You can view my homework assignment 1 using the  above link. All 3 pages (Introduction, CS Department Info and Survey Pages) along with their CSS files and other media are uploaded to the AWS S3 bucket.

Steps followed to host on AWS S3:

Created an AWS free tier account and created a S3 bucket.
Unchecked the disable public access while doing so.
Under properties - enable static website hosting and save changes
under permissions - enable public access and add bucket policy wherein added bucketname under Resource (from the tutorial given)
Uploaded all files mentioned above to the bucket created
Tested the above link and is working.

Part 2 

EC2 :

Note: If you click on the below link and it may show "Your connection is not private.", you can move ahead to view this website  by clicking  on "Advanced " and clicking "Proceed to address(unsafe)" , in Chrome browser , and you will be able to view the website.


Please check out my assignment below hosted on AWS EC2 :
http://ec2-3-89-250-86.compute-1.amazonaws.com

Steps followed to host on AWS EC2 :
1. Created an EC2 instance and added key-value pair 
2. Checked Allow HTTPS and HTTP traffic from the internet
3. Click on Launch instance 
4. Start the instance and wait for status check to be "2/2 test cases passed "
5. Click on Connect and under "EC2 instance connect" click connect 
6. Now, as the terminal appears, follow these steps:
sudo su -          // move to root 
yum update -y 
sudo yum install -y httpd    //For Amazon Linux
mkdir swe642-assignment1 
cd swe642-assignment1
wget "Enter the Zip file link address of your complete code"
unzip the file 
mv * /var/www/html/             //Move your files to Web Server Directory 
cd  /var/www/html/
Now, your Web server has your website 
systemctl enable httpd
systemctl start httpd        // Start the httpd web server 
Now you can run your website my clicking on our Public IPv4 address or Public IPv4 DNS 
Tested the above link and is working.

