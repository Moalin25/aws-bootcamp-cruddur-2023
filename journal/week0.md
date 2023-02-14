# Week 0 — Billing and Architecture!

# Locgical Diagram

The purpose of this diegram is show case a pipeline in where we as the developers create a dockerfile and push it into our repo. Where the pipeline will be triggered on a push to main. The code build will pick up the newly commited dockerfile and use the build spec to produce a docker imagie. Then code deploy will use the built docker imagie to deploy the application on an ec2 which will be managed by ECS. Users will be able to acces our application visa DNS where traffic will be routed to the Application Load Balancer and on to the Instances.

![Screenshot 2023-02-14 at 16 17 39](https://user-images.githubusercontent.com/124910763/218805474-de8f070f-1763-4fd0-8a0e-f9e8f01ffa61.png)

# Conceptual Diagram
![Screenshot 2023-02-14 at 16 56 33](https://user-images.githubusercontent.com/124910763/218805289-2eeb8706-8dc9-49a8-a080-e683d5b7e4d8.png)

# CloudWatch Alarm Config Json File
![Screenshot 2023-02-14 at 16 21 17](https://user-images.githubusercontent.com/124910763/218797469-e89052ff-02b5-4713-bdb7-22082cdf3b5a.png)

# Budget Alarm Config Json File
![Screenshot 2023-02-14 at 16 24 45](https://user-images.githubusercontent.com/124910763/218797741-5def7dd5-1e2e-4c55-879a-518d89a50525.png)

# Sns Subcription Json File
![Screenshot 2023-02-14 at 16 24 58](https://user-images.githubusercontent.com/124910763/218797985-4126e273-5e42-46b3-94b3-d2ee95161293.png)
