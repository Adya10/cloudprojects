This is a step by step guide of how to make a VPN server in AWS

Step 1.

a. Go in amazon console and search for EC2

b. Launch a new instance with an AMI from amazon market place.

c. In amazon market place search for openvpn and press enter.

d. Scroll a bit until you find free tier eligible AMI

e. Select that AMI

<img width="1440" alt="Step 1" src="https://github.com/Adya10/cloudprojects/assets/82889880/b16c9ac1-fb21-4858-a369-a9a84b3c63f9">

Step 2.

a. Once you've selected an AMI, select t2.micro as your instance type.

<img width="1440" alt="Step 2" src="https://github.com/Adya10/cloudprojects/assets/82889880/7028c8b8-fcb4-4a0f-8734-cffc4644f505">

Step 3.

a. For the security group, a new security group will be created and you can leave the settings as it is.

b. For the key pair you can create a new key pair or you can select an existing one if you already have one.

Step3 photo

Step 4.

a. Once your instance is created ssh into your instance, you will be promted to login as "openvpnas" instead of "root"

Step4 photo

Step 5.

a. Modify the command to login as "openvpnas"

b. Accept the certificate.

c. Keep all the settings as default.

d. Set a new password for user "openvpn" when prompted.

Step 5 photo

Step 6.

a. Copy the public ip address of your instance.

Step 6 photo

Step 7.

a. In the new tab type https://"publicipofyourinstance":943/admin

b. The username is openvpn and the password is the one you set earlier

step 7 photo

c. Once you login, you're the admin so you can change the settings as you like.

Step7.2

Step 8. (Optional)

a. The one setting I changed here is all the client internet traffic will be routed through this vpn when connected.

b. To do that on left hand side, drop down the configuration tab and press on VPN settings.

c. You’ll see "Should client Internet traffic be routed through the VPN?" turned to NO. Toggle that to YES.

Step 8

Step 8.2

d. At the bottom of the page press save settings and then at the top of page press "Update Running Server"

Step 8.3

Step 9.

a. Now go to the url again and remove /admin/vpn_settings and press enter. You'll be redirected to another login page.

b. The username is openvpn and password is the one you set earlier.

Step9

Step 10.

a. Download the file on your desired platform.

Step 10

Step 11.

a. Once the download is complete open the file and accept the terms, and login with same username and password. You can now connect to your vpn.

Step11
