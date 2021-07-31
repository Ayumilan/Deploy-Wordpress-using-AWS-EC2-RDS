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

# Set up the RDS database on AWS

As wordpress stores data at the backend in MySQL Database server. Therefore, setup a MySQL server using AWS RDS service using Free Tier
follow the steps

![18](https://user-images.githubusercontent.com/60690689/127743209-0a72aaba-1bae-47dd-afcd-8ff58a2c8170.jpg)
![19](https://user-images.githubusercontent.com/60690689/127743221-72ac5072-3815-49a1-bf38-50310dcc7354.jpg)
![20](https://user-images.githubusercontent.com/60690689/127743230-cccdcd10-ca4c-4661-993f-33e2f5991b3a.jpg)
![21](https://user-images.githubusercontent.com/60690689/127743239-ab8fad21-dfde-43ce-ba31-dc3986d80734.jpg)
![22](https://user-images.githubusercontent.com/60690689/127743243-8ac58bcd-30aa-41b2-b49d-e63f7582221c.jpg)
![23](https://user-images.githubusercontent.com/60690689/127743258-d0c0badc-44c2-4a51-886e-9cee0a612bc2.jpg)
![24](https://user-images.githubusercontent.com/60690689/127743263-ed3ec054-4419-4f82-8ce0-9ec43ef9e6eb.jpg)

Our RDS is created

![25](https://user-images.githubusercontent.com/60690689/127743285-a780bc1f-3d03-4f63-8ff6-b6629c04dbbb.jpg)

# Steps to provide the endpoint/connection string to the WordPress

![26](https://user-images.githubusercontent.com/60690689/127743353-de911463-9f9e-4728-9566-f700fc0cf963.jpg)
![27](https://user-images.githubusercontent.com/60690689/127743360-308b4634-84ab-432a-bd6d-c05f33424775.jpg)

here we see, we are unable to connect to the database we have to change some inbound rule in security group 

![28](https://user-images.githubusercontent.com/60690689/127743408-a29e2af6-3e1b-44bc-be08-03c19a0b150e.jpg)

Again connect with the database...

![29](https://user-images.githubusercontent.com/60690689/127743429-8639a640-3cbd-4273-b628-0ebbd382cf1a.jpg)
![30](https://user-images.githubusercontent.com/60690689/127743438-fd4685cd-bb4b-4a66-80fa-88f9417176c6.jpg)
![31](https://user-images.githubusercontent.com/60690689/127743459-1b271824-8aa9-4ec2-8252-efd93f8c091d.jpg)
![32](https://user-images.githubusercontent.com/60690689/127743463-d5bb459c-fd1c-46f0-bb1d-ef06976b4df3.jpg)

Now we have to Set up the config file ..

![33](https://user-images.githubusercontent.com/60690689/127743487-122906b8-433e-4c88-b3d7-0af0a06607cb.jpg)
![34](https://user-images.githubusercontent.com/60690689/127743495-c169f304-2dd4-4fba-8609-eed2781d87b8.jpeg)

Let's Login to the wodpress site ...

![35](https://user-images.githubusercontent.com/60690689/127743515-de071077-902d-4adc-99b6-bc8808f574e9.jpg)
![36](https://user-images.githubusercontent.com/60690689/127743520-cefc7a3f-ba8b-4c4a-94aa-d04dbe3f21de.jpg)
![37](https://user-images.githubusercontent.com/60690689/127743534-239c5b80-0398-42f0-b69a-e8b496bc738a.jpg)

#### THANK YOU
