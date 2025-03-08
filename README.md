# Host-a-Website-on-Amazon-S3
Hosting a Static website on internet - Can be a portfolio 

You can use Amazon S3 to store and retrieve any amount of data at any time from anywhere on the web.
In this Case, I used amazon S3 service which is (Amazon Simple Storage Service)
go to amazon management console which AWS account and type S3 services, 
![S3 service](https://github.com/user-attachments/assets/08f219eb-10ce-48ac-8e8e-c0dd5c78d566)
Select the region on top right corner to use the closet data center to your location. The region i picked for my S3 bucket was Asia pacific (Mumbai) because it allows compliance with local data residency requirements ensuring faster data transmission and low latency issues, and Mumbai is the closet place to me

Make sure that you give unique name to your S3 bucket as, no two S3 buckets can have same name globally accross ALL AWS accounts. This prevents conflicts and confusion especially when multiusers are working with AWS services
![S3](https://github.com/user-attachments/assets/3dd8eeca-82e9-4513-a17c-35242fc536dd) - My project name was nextwork-website-project-vishal as i was building my personal portfolio
while setting up your S3 bucket you will come across few policies like object ownerships - nothing but the owner or S3 service, ACL's list - getting access to your S3 bucket publicly to the multi user's who will be working with AWS services within the company, if you want ACl to be a little briefed here it is, 
ACL: ACCESS CONTROL LISTS which is a set of rules that defines permissions for accessing resources in a computing environment.allowing users to control access to their data based on their specific needs and security requirements.
![ACL's](https://github.com/user-attachments/assets/32477a9f-cbab-4088-a9b6-45fde71eb74b)
You have to uncheck block all public access and ackownledge "that the current settings might result in this bucket and the objects within becoming public". Because this will allow to get S3 bucket visible within the organization. 

Upload website content to your bucket

an HTML file that sets up your website: This involves the portfolio or anything that you work within HTML extensions

a zip file of images for your website: This involves, either your portfolio image or any other contents, make sure that you unzip files cause, without unzipping S3 bucket cannot read the contents directly

Upload both files into your S3 bucket.
![S3 Docs upload](https://github.com/user-attachments/assets/e802dc7d-78a1-42e7-965d-a20e6f12cb3d)

Now once, the files are uploaded, host this static webiste from S3 bucket, choose enabled option to be live on the internet and then save it, so it would be like this 
![Host S3](https://github.com/user-attachments/assets/61fc4102-04a3-4937-ad2e-d2ed8daabe88)
this will generate a URL on the bottom of the screen once the changes are saved, you might get an error like while accessing the link
![S3 block](https://github.com/user-attachments/assets/fa79f4b3-aaab-4038-8eaa-f2c7fce6a516), this could be because you need to enable your content inside the folder using manage ACL list under actions tab, this will allow your site and it's content to be accessed on internet publicly.

After the change you can refresh your link and your static website is live now. 
![S3 project](https://github.com/user-attachments/assets/45a65370-8d9c-44a4-97e2-63be318a4a53)
