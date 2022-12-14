# Aws-beanstalk-example
aws-beanstalk-example : API that will use a string as input and does a find and replace for certain words and outputs the result. For example: replace Google for Google©
# What's Here
buildspec.yml - this file is used by AWS CodeBuild to build the web application     
pom.xml - this file is the Maven Project Object Model for the web application      
src/main - this directory contains your Java service source files     
src/test - this directory contains your Java service unit test files    
 
# Aws Service used in development 
# Code Pipeline -
 Code Commit,Code build, Code Deploy
# Elastic beanstalk - Paas
  To deploy application.
  
# Request - 
curl --location --request POST 'http://test2-env-1.eba-3x7gpdvh.us-east-1.elasticbeanstalk.com/append-copyright-symbol' \
--header 'Content-Type: text/plain' \
--data-raw '"We really like the new security features of Amazon Cloud"'

# Response -
"We really like the new security features of Amazon© Cloud"

# What is next  - Serverless 
Elastic Beanstalk is great, it handles the deployment,capacity provisioning, load balancing, auto-scaling, and health monitoring but still you are paying for resource when your application is not running so It serverless solution for this usage case should be ideal.

