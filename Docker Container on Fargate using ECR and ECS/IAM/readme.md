You need to create an IAM role so that your EC2 instance can talk to ECR. Follow these to steps to crete the appropriate IAM role.

Step 1

a. Go to services in AWS management console and search 'IAM'.

b. On the left panel click on 'Roles' and press on 'Create role'

![Step 1](https://github.com/Adya10/cloudprojects/assets/82889880/651b11a5-0213-404a-89b8-2d293259f0d3)

Step 2

a. Select AWS service as trusted entity type and select EC2 as common use cases.

![Step 2](https://github.com/Adya10/cloudprojects/assets/82889880/1cbdfbc7-985d-4183-8be0-5decd573bf9e)

Step 3

a. Search for AmamzonEC2ContaniverRegistryFullAccess and select the policy.

b. Once the poilicy is selected click on next.

![Step 3](https://github.com/Adya10/cloudprojects/assets/82889880/e42f0834-aa48-4c79-9311-8680607fe9e3)

Step 4

a. Give the appropriate name to your role and select create role.

![Step 4](https://github.com/Adya10/cloudprojects/assets/82889880/8199f442-bb53-4d9f-85f6-4ee7139633a0)
