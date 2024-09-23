Workload name: Tomcat

Support OS: Linux

Workload Version: 9.0.33

Dependency: OpenJDK-8.1.10.3, Go-1.10.3

# Docker Image ID: 
    Parent Image: tomcat:9.0.33-jdk8


# Steps to create custom image:

docker build -t tomcatgobin:9.0.33 .

# Docker commands:

To Push Custom Image to Docker Repo

Step 1 : docker login
Step 2 : docker tag tomcatgobin:9.0.33 <docker hub Username>/tomcatgobin:9.0.33
Step 3 : docker push <docker hub Username>/tomcatgobin:9.0.33
Step 4 : docker pull <docker hub Username>/tomcatgobin:9.0.33
Step 5 : docker run -it -d --name ApacheTomcat9033 -p 8080:8080 <docker hub Username>/tomcatgobin:9.0.33
