# Week 0 — Billing and Architecture!

# Locgical Diagram

The purpose of this diagram is show case a pipeline in where we as the developers create a dockerfile and push it into our repo. The pipeline will be triggered on a push to main. Codebuild will pick up the newly commited dockerfile and use the build spec file to produce a docker imagie. Then Codedeploy will use the built docker imagie to deploy the application on an ec2 which will be managed by ECS. Users will be able to acces our application visa DNS where traffic will be routed to the Application Load Balancer and on to the Instances.

![Screenshot 2023-02-14 at 16 17 39](https://user-images.githubusercontent.com/124910763/218805474-de8f070f-1763-4fd0-8a0e-f9e8f01ffa61.png)

# Conceptual Diagram
![Screenshot 2023-02-14 at 16 56 33](https://user-images.githubusercontent.com/124910763/218805289-2eeb8706-8dc9-49a8-a080-e683d5b7e4d8.png)

# Budget Alarm 

Created an aws budget alarm 
![Screenshot 2023-02-16 at 18 26 29](https://user-images.githubusercontent.com/124910763/219455109-503a1bf2-1b66-481a-8555-4f85bfccf86b.png)

