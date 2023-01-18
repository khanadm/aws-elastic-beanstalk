
 #### What is Elastic Beanstalk ?
---

Elastic Beanstalk is a service for deploying and scaling web applications and services. Upload your code and Elastic Beanstalk automatically 
handles the deployment—from capacity provisioning, load balancing, and auto scaling to application health monitoring.

---

In this we have two  Environment  
---
 
 
### 1. Websever Environment
 
    
A web server is software and hardware that uses HTTP (Hypertext Transfer Protocol) and other protocols to respond to client requests made over the 
World Wide Web. The main job of a web server is to display website content through storing, processing and delivering webpages to users.
 
### 2. Worker Environment


The worker environment SQS daemon Worker environments run a daemon process provided by Elastic Beanstalk. This daemon is updated regularly to 
add features and fix bugs.
 
---


### **Note:** 
1. EB CLI configuration requires AWS Credentials, Click [Understanding and getting your AWS credentials.](https://docs.aws.amazon.com/general/latest/gr/aws-sec-cred-types.html#access-keys-and-secret-access-keys)
2. Refer [EB CLI Basics.](https://docs.aws.amazon.com/elasticbeanstalk/latest/dg/eb-cli3-getting-started.html#ebcli3-basics-create)
3. The signup-webserver directory has a file named **iam_policy.json**. Copy this policy to the attached [IAM role](https://docs.aws.amazon.com/IAM/latest/UserGuide/id_roles.html) so that the instance can access Dynamo DB and SNS Services. 
4. Don't forget to change the **email address** in `setup.config` file under `.ebextensions directory of signup-webserver`.


---


Let's configure webserver Environment


![1](https://user-images.githubusercontent.com/106643382/213102906-d08d77d4-3eab-4f30-b33e-12b7d8e89c47.png "1")

![2](https://user-images.githubusercontent.com/106643382/213103097-5ef44812-fa0d-474b-83c7-c816e203df16.png "2")

![3](https://user-images.githubusercontent.com/106643382/213103181-8352c1d3-f65e-42f1-b9cd-3caf16c19d75.png "3")

And lastly upload your code in webserver.



























