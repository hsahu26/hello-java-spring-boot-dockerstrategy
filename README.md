# hello-java-spring-boot

This is a simple Spring Boot application, which displays some information to the user, about _cheese_. The exact type of cheese that is displayed, is set via configuration. Thus demonstrating the power of Spring Boot configuration properties, and how you can override them at runtime.

🎥 There's a YouTube video to accompany this repo: <https://www.youtube.com/watch?v=5Fphv4lVrmU>


What will be flow -

This example expect Openshift will use integrated jenkins that will be using openshift-plugin

1. create secret with sshprivate key and deploy ssh public key on sepecific repo (not in user profile)
2. create build config which will use jenkinspipeline strategy that will create jenkins job automatically and refer jenkinsfile to proceed further, this build config is enabled for github trigger so it will be triggered once repo updated
3.  create build config which will be using docker build strategy to take instruction from dockerfile by using binary build, this build config will be called by jenkins file stage.
4. So build is ready and that can be deployed and exposed 

