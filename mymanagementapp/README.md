This is a simple web application used to manage corporate processes. It includes options for adding, completing, and deleting tasks, as well as reporting the overall number of tasks. This README.md file describes how to run the program locally, create a Docker image, and launch a container from the image.
To run the application locally;git clone <repository-url>
Navigate to the project directory;cd business-management-application
Open the index.html file in a web browser to access the application.



To build the Docker image and run a container using the image;
Ensure Docker is installed on your machine
Navigate to the project directory containing the Dockerfile
Build the Docker image using the following command:
FROM nginx:alpine

COPY . /usr/share/nginx/html

EXPOSE 80

CMD ["nginx", "-g", "daemon off;"]
