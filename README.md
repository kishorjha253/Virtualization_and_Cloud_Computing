# Virtualization_and_Cloud_Computing
Assignment and code for Virtualization and Cloud Computing
This repository contains a simple Python Flask web application that can be easily deployed using Docker.

Functionality

  The Flask application in this project serves a single endpoint:

	1) Add Notes: Provide an option to add notes in the web application.
	2) View notes: Display all the provided notes in the web application.



Prerequisites

   Before you begin, ensure you have the following installed on your system:

	- Docker: [Docker Installation Guide](https://docs.docker.com/get-docker/)

Getting Started

  Follow these steps to deploy the Flask application using Docker:

  1. Clone the Repository:

   >>shell

   $git clone https://github.com/kishorjha253/Virtualization_and_Cloud_Computing.git

   $cd Virtualization_and_Cloud_Computing
   
  2. Build the Docker Image:
   Build the Docker image using the provided Dockerfile
   
   $ docker build -t my-flask-app .
   
   Replace my-flask-app with your desired image name.

  3. Run the Docker Container:
   Run a Docker container from the built image, mapping port 5000 from the container to your host machine
   
   $ docker run -d -p 5000:5000 my-flask-app
   
   The Flask application will be accessible at http://localhost:5000 in your web browser.
   
  4. To Stop the docker container
     check the running container list
	 $ docker ps
	 $ docker stop <container_name_or_id>

Usage
   Access the Flask application by opening your web browser and navigating to http://localhost:5000. 
   You should see the "sample Web application" page and use its functionality.
   
Customization
	You can customize the Flask application by modifying the app.py file. 
	Add more routes, templates, or functionality as needed.
	To install additional Python packages, update the requirements.txt file and rebuild the Docker image.

Contributing
    Contributions are welcome! If you have improvements or suggestions, please open an issue or create a pull request.

License
     This project is licensed under the MIT License. See the LICENSE file for details.
     The project is a part of IIT jodhpur assignment1. 
	 
Author Details:
    Name : Kishor Kumar
    Email : kumar.253@iitj.ac.in
    Roll : M20AIE245

