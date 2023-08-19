## assignment2_part1

## Step 1 Create a new Docker network named "my_network" using the bridge driver. (2 marks)
```
docker network create my_network
```
![image](https://github.com/mwaqaskh/assignment2_part1/assets/39801941/13affeae-9290-4b11-aa19-bf256da95c62)
![image](https://github.com/mwaqaskh/assignment2_part1/assets/39801941/87f37827-c237-40ea-a60e-a30196a74b18)

## Step 2 Create a new Docker container using the "nginx" image and connect it to the "my_network" network. Name the container "nginx_container". (4 marks)
```
docker run -d --name nginx_container --network my_network -p 8080:80 nginx
```

![image](https://github.com/mwaqaskh/assignment2_part1/assets/39801941/f0fb0c5f-8aa9-4326-8803-c4c03cd00e64)


## Step 3 Verify that the "nginx" default page is accessible on your host machine at http://localhost:8080. (2 marks)

![image](https://github.com/mwaqaskh/assignment2_part1/assets/39801941/6778bb05-b920-4e01-9156-4cb47864534a)


## Step 4 Create a new Docker container using the "httpd" image and connect it to the
"my_network" network. Name the container "httpd_container". (4 marks)
# Step 5 Verify that the "httpd" default page is accessible on your host machine at
http://localhost:8081. (2 marks)
## Step 6 Use the "docker network inspect" command to display information about the
"my_network" network. Document your findings in the README.md file. (4 marks)
## Step 7 Stop and remove the "nginx_container" container. (2 marks)
## Step 8 Create a new Docker container using the "nginx" image and connect it to the
"my_network" network. Name the container "nginx_container_2". (4 marks)
## Step 9 Verify that the "nginx" default page is accessible on your host machine at
http://localhost:8082. (2 marks)
## Step 10 Use the "docker container ls" command to display information about all running
containers. Document your findings in the README.md file. (4 marks)
## Step 11 Stop and remove all containers. (2 marks)
## Step 12 Cleanup: Remove the "my_network" network. (2 marks)
## Step 13 Create a README.md file and document your findings for each command. For each
command, provide a brief description of what it does, followed by the output and logs
generated by the command. Ensure that the README.md file is well-organized, easy to
read, and contains all necessary information. (18 marks)
## Step 14 Push the codebase for the sample application to your GitHub repository (create a new
one for this part)
