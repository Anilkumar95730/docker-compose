
# DOCKER COMPOSE:
          	It is a tool used to build, run and ship the multiple containers for application.  
            It is used to create multiple containers in a single host.
          	It used YAML file to manage multi containers as a single service.
     	  The Compose file provides a way to document and configure all of the application’s service dependencies (databases, queues, caches, web service 
            APIs, etc).

# COMMANDS:
                   Start all services: Docker Compose up. 
                   Stop all services: Docker Compose down.
                   Run Docker Compose file: Docker-compose up -d.
                   List the entire process: Docker ps.

create a EC2 instance on Linux and connect to it.

Now install the Docker and Start it.

Now Paste command of Compose installation in curl in the form of

                           sudo curl -L https://github.com/docker/compose/releases/latest/download/docker-compose-$(uname -s)-$(uname -m) -o /usr/local/bin/docker-compose.
                          
                          
And Give the excute  permissions 

                         (Chmod +x /usr/local/bin/docker-compose)
Check the version of docker compose by using 

                             docker-compose --version
Create the docker compose file by using command

                            vi docker-compose.yaml 
                            
Docker compose file
![Screenshot 2024-11-07 174503](https://github.com/user-attachments/assets/51461736-fc0f-4f50-81f5-8c935f9dd979)

Execute or start the docker compose file by using
                           docker-compose up or docker-compose up -d command.

Diff b/w compose up and compose up -d is when we use docker compose up command it will create ,start and stop or existed state the container immediately whereas docker-compose up -d command is create ,start and continuously running the container.r 


![Screenshot 2024-11-07 174719](https://github.com/user-attachments/assets/6ac8b74b-1675-48a5-8633-94966f01b065)

# After that edit the security group of inbound rules
![Screenshot 2024-11-07 174636](https://github.com/user-attachments/assets/77c8e934-7af0-41b3-9c96-8e0ba9f7c774)

# Access the NGINX
![Screenshot 2024-11-07 174320](https://github.com/user-attachments/assets/74d52269-e331-483a-987f-ccb0c1ad19c8)
# Access the httpd
![Screenshot 2024-11-07 174656](https://github.com/user-attachments/assets/148cbb63-5207-4e71-8d18-4170a6ae5a43)

By using the docker custom image from docker hub we can create and run the container.

First log into our docker hub and we can configure the docker on the ec2 instance or server by using docker login command.

Enter username and password.
![Screenshot 2024-11-07 180932](https://github.com/user-attachments/assets/0ebb6d0f-2f65-42e5-8855-2759f9c09b82)


Open docker compose file which we have created earlier and add the service name like below image.

![Screenshot 2024-11-07 181948](https://github.com/user-attachments/assets/7dac5016-8cef-44e3-a6c5-ac888abe868a)


Start the docker compose file by using docker-compose up -d command.

![Screenshot 2024-11-07 174719](https://github.com/user-attachments/assets/e08065f3-8dd6-48b4-9ab7-5cc249175c91)
# Access the application
![Screenshot 2024-11-07 182116](https://github.com/user-attachments/assets/0f199d50-2920-4251-a4bb-263923f9a8e9)
