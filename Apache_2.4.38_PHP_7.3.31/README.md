Workload name: Apache with PHP

Support OS: Debian 10

Workload Version: 
Apache - 2.4.38

Dependency: PHP - 7.3.31

# Steps to create custom image:

docker build -t apache24php:7.3.31 .

# Docker commands:

To Push Custom Image to Docker Hub

Step 1 : docker login

Step 2 : docker tag apache24php:7.3.31 \<docker hub Username\>/apache24php:7.3.31
    
Step 3 : docker push \<docker hub Username\>/apache24php:7.3.31

    
# To Pull Custom Image from Docker Hub
Step 4 : docker pull \<docker hub Username\>/apache24php:7.3.31

# Create Tomcat Container
Step 5 : docker run -it -d --name ApachePHP -p 80:80 \<docker hub Username\>/apache24php:7.3.31

