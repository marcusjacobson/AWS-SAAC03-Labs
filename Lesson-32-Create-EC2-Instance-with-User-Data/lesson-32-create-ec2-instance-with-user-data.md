# Launch EC2 Instance

1. From the EC2 console, launch a new Amazon Linux instance.

![new-instance-1](/Lesson-32-Create-EC2-Instance-with-User-Data/images/new-instance-1.png)

2. Select the instance type of T2-micro (free tier).

![new-instance-2](/Lesson-32-Create-EC2-Instance-with-User-Data/images/new-instance-2.png)

3. Create a new key pair, to allow for SSH connectivity.

![new-instance-3a](/Lesson-32-Create-EC2-Instance-with-User-Data/images/new-instance-3a.png)

![new-instance-3b](/Lesson-32-Create-EC2-Instance-with-User-Data/images/new-instance-3b.png)

![new-instance-3c](/Lesson-32-Create-EC2-Instance-with-User-Data/images/new-instance-3c.png)

4. Configure network settings to allow SSH and HTTP traffic, since this willb e for a basic Web server.

![new-instance-4](/Lesson-32-Create-EC2-Instance-with-User-Data/images/new-instance-4.png)

5. Expand the Advanced settings and scroll to user data. Add in the user data code from the provided course download.

**Note**: This user data configured a simple Apache web server.

![new-instance-5](/Lesson-32-Create-EC2-Instance-with-User-Data/images/new-instance-5.png)

All other settings will remain as default. Once the User Data is added, select **Launch instance**.


# Test Web Server Functionality

1. Select the running instance and copy the public IPv4 address.

**Note**: Selecting the **open address** link will launch the HTTPS instance, which we are not cofigured for at this time.

![test-web-server-1](/Lesson-32-Create-EC2-Instance-with-User-Data/images/test-web-server-1.png)

2. Open a new browser tab and paste IPv4 address. If it loads succesfully it will appear as:

![test-web-server-2](/Lesson-32-Create-EC2-Instance-with-User-Data/images/test-web-server-2.png)