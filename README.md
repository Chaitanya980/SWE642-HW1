This assignment contains:

A index.html page - Has my personal Introduction page with a picture and brief description about myself. A student class Webpage. It contains links to CS Department Information page and Studnet Survey Form . You can find the button link on top at the header section of this page.

A department.html - A CS Department Information page. With two paragraphs, a MS degrees List and the required courses as per each degree table. It also links to the student survey form page. You can find the button link on top at the header section of this page.

A survey.html - It has a student survey form made keeping in mind all the requirements mentioned on the assignemnt question. Facility has been given to navigate from any of the 3 pages to the others.

An images folder - which contains images  used for this assignment.

bootstrap.min.css and bootstrap.min.js files

A readme.md file

Styling sheets(department.css, style.css and survey.css) for all the 3 pages 

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