## Dockerized Flask App
This project demonstrates how to convert a simple Flask web application written in Python into a Docker image.

### Flask Overview
Flask is a lightweight web framework for Python, making it one of the simplest ways to build web applications. It’s great for getting a web application up and running quickly with minimal setup.

![Screenshot (316)](https://github.com/user-attachments/assets/842c032c-9fdd-4c26-b0fa-5d4eff6927f6)

![Screenshot (319)](https://github.com/user-attachments/assets/ad5f88e0-5e14-4490-bc6a-3465a1fbdf75)


### Building the Docker Image
To create the Docker image for the Flask app, I used the following command:   
docker build -t ruwanthilakshika/hey-python-flask:0.0.1.RELEASE .     

![Screenshot (314)](https://github.com/user-attachments/assets/023b970f-aeb3-4ee2-8bf6-c9b7b1196ca3)

### Running the Docker Image
To run the Docker image and map it to port 3000, I used:        
docker container run -d -p 3000:3000 ruwanthilakshika/hey-python-flask:0.0.1.RELEASE        

![Screenshot (315)](https://github.com/user-attachments/assets/d1431b6c-d211-4c63-8e73-219c56b1016a)

### Changing the Running Port
If you need to change the port that the container is running on, you can do so with:     
docker container run -d -p 4000:3000 ruwanthilakshika/hey-python-flask:0.0.1.RELEASE         

![Screenshot (318)](https://github.com/user-attachments/assets/f60b087b-eacc-437d-a635-c43ddaa3253c)

### Pushing the Image to Docker Hub
To share this Docker image, I pushed it to Docker Hub using:       
docker push ruwanthilakshika/hey-python-flask:0.0.1.RELEASE        

![Screenshot (320)](https://github.com/user-attachments/assets/8c1fe1ea-9652-47dd-b197-a5efb0f8d58f)







