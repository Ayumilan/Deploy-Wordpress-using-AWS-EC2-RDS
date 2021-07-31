# Deploy-Wordpress-using-AWS-EC2 & RDS

🔅 Create an AWS EC2 instance

🔅 Configure the instance with Apache Webserver.

🔅 Download php application name “WordPress”.

🔅 As wordpress stores data at the backend in MySQL Database server. Therefore, setup a MySQL server using AWS RDS service using Free Tier.

🔅 Provide the endpoint/connection string to the WordPress application to make it work.

# Steps To Launch An EC2 Instance

Go to your AWS console and launch an instance. follow the ScreenShot
![1](https://user-images.githubusercontent.com/60690689/127742745-47cfdb7f-48cb-45d7-a72b-bad93bdcd6b7.jpg)
![2](https://user-images.githubusercontent.com/60690689/127742762-7537cd89-18db-49cd-81d1-b566c82fb18f.jpg)
![3](https://user-images.githubusercontent.com/60690689/127742764-4d0770d2-48e0-4508-9727-fd5c1a3c4267.jpg)
![4](https://user-images.githubusercontent.com/60690689/127742776-af8501b6-8ee0-446e-a19b-ab264f090038.jpg)
![5](https://user-images.githubusercontent.com/60690689/127742779-e26d7872-2179-4690-a3a0-cce3681fb087.jpg)
![6](https://user-images.githubusercontent.com/60690689/127742786-52fb524b-dc63-4353-95b8-97b610393ebe.jpg)
![7](https://user-images.githubusercontent.com/60690689/127742793-e894fd36-36eb-45c5-8b6a-9f53d75e4414.jpg)
![8](https://user-images.githubusercontent.com/60690689/127742796-be5926d7-87a7-4ffb-8e0b-82c2c3ba9fab.jpg)
![9](https://user-images.githubusercontent.com/60690689/127742802-e085e942-963a-4f76-aeab-85a8d3b82018.jpg)

Our Instance has launched.

![10](https://user-images.githubusercontent.com/60690689/127742820-763a0603-8bf3-4a1a-b181-14b6a34b621d.jpg)

# Steps to configure the instance with Apache Webserver

Open the Instance in putty and configure it.
Install httpd, vim, php, wget

![11](https://user-images.githubusercontent.com/60690689/127742972-cb30ddbe-b748-46f2-b5eb-b3a6a62da93c.jpg)
![12](https://user-images.githubusercontent.com/60690689/127742976-2edc12c0-4267-4cec-9c6e-142e3137a966.jpg)
![13](https://user-images.githubusercontent.com/60690689/127742983-a2af7122-814c-4f65-ad4f-a122d756e5bd.jpg)

# Steps to download php application name “WordPress”

![14](https://user-images.githubusercontent.com/60690689/127743022-a67784ab-5171-43f9-bf19-1783336862f0.jpg)

untar the file and copy it in /var/www/html  folder

![15](https://user-images.githubusercontent.com/60690689/127743053-932fd28a-4cbe-4316-a369-23bb9b2fe401.jpg)

Check the httpd service status 

![16](https://user-images.githubusercontent.com/60690689/127743080-586a57b2-c530-44db-9170-c40297566844.jpg)

Check the website with the instance ip

![17](https://user-images.githubusercontent.com/60690689/127743104-c5165921-d258-4584-aafd-82aa077ea56b.jpg)

Here we need a database to save our data, we have to set up a database.
