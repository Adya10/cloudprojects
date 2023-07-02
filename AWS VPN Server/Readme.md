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

<img width="1440" alt="Step 3" src="https://github.com/Adya10/cloudprojects/assets/82889880/93f3a051-6a7e-4383-9414-a3cb831e399f">

Step 4.

a. Once your instance is created ssh into your instance, you will be promted to login as "openvpnas" instead of "root"

<img width="1440" alt="Step 4" src="https://github.com/Adya10/cloudprojects/assets/82889880/95fdf7c2-a79a-4867-9786-d1eca8f26208">

Step 5.

a. Modify the command to login as "openvpnas"

b. Accept the certificate.

c. Keep all the settings as default.

d. Set a new password for user "openvpn" when prompted.

<img width="1440" alt="Step 5" src="https://github.com/Adya10/cloudprojects/assets/82889880/c1ece77f-78de-4209-a5a2-f6648766ab0a">

Step 6.

a. Copy the public ip address of your instance.

<img width="1440" alt="Step 6" src="https://github.com/Adya10/cloudprojects/assets/82889880/a4379fdc-bd26-452e-b799-c040cd50bd9b">

Step 7.

a. In the new tab type https://"publicipofyourinstance":943/admin

b. The username is openvpn and the password is the one you set earlier

<img width="1440" alt="Step 7" src="https://github.com/Adya10/cloudprojects/assets/82889880/8ac641e2-01cf-402a-a7e4-3f84a68d69d8">

c. Once you login, you're the admin so you can change the settings as you like.

<img width="1440" alt="Step 7 2" src="https://github.com/Adya10/cloudprojects/assets/82889880/8b728e0f-b043-4793-bdbc-30108dc88ec4">

Step 8. (Optional)

a. The one setting I changed here is all the client internet traffic will be routed through this vpn when connected.

b. To do that on left hand side, drop down the configuration tab and press on VPN settings.

c. You’ll see "Should client Internet traffic be routed through the VPN?" turned to NO. Toggle that to YES.

<img width="1440" alt="Step 8" src="https://github.com/Adya10/cloudprojects/assets/82889880/1c8debe8-8a8a-403a-bcab-0982b61e192c">

<img width="1440" alt="Step 8 2" src="https://github.com/Adya10/cloudprojects/assets/82889880/4ffe3b25-1ec8-48d0-b9b8-cde01e3d10a5">

d. At the bottom of the page press save settings and then at the top of page press "Update Running Server"

<img width="1440" alt="Step 8 3" src="https://github.com/Adya10/cloudprojects/assets/82889880/1d598604-521f-4869-a7a9-2566bc2aad2a">

Step 9.

a. Now go to the url again and remove /admin/vpn_settings and press enter. You'll be redirected to another login page.

b. The username is openvpn and password is the one you set earlier.

<img width="1440" alt="Step 9" src="https://github.com/Adya10/cloudprojects/assets/82889880/024ac74b-f58b-4396-97bd-c86d8e5625f7">

Step 10.

a. Download the file on your desired platform.

<img width="1440" alt="Step 10" src="https://github.com/Adya10/cloudprojects/assets/82889880/eaf24d9e-25e5-4453-beca-d0c0e364242c">

Step 11.

a. Once the download is complete open the file and accept the terms, and login with same username and password. You can now connect to your vpn.

<img width="1440" alt="Step 11" src="https://github.com/Adya10/cloudprojects/assets/82889880/e2b292f8-bcb1-4483-91c2-c3bae61b4856">
