# Inception: Mastering System Administration with Docker Virtualization!

|    Project Name    |                                                                       inception                                                                      |
| :----------------: | :-------------------------------------------------------------------------------------------------------------------------------------------------: |
|    Description     |       This project aims to enhance understanding of system administration through the utilization of Dockerfile for creating and managing custom images and microservices.                                       |
|    Technologies    | <a href="#"><img alt="Docker" src="https://img.shields.io/badge/docker-%230db7ed.svg?style=for-the-badge&logo=docker&logoColor=white"></a> <a href="#"><img alt="Nginx" src="https://img.shields.io/badge/nginx-%23009639.svg?style=for-the-badge&logo=nginx&logoColor=white"></a> <a href="#"><img alt="Wordpress" src="https://img.shields.io/badge/WordPress-%23117AC9.svg?style=for-the-badge&logo=WordPress&logoColor=white"></a> <a href="#"><img alt="HTML" src="https://img.shields.io/badge/HTML-E34F26.svg?logo=html5&logoColor=white&style=for-the-badge"></a> <a href="#"><img alt="MariaDB" src="https://img.shields.io/badge/MariaDB-003545?style=for-the-badge&logo=mariadb&logoColor=white"></a> |

##### Prerequisite

To run the project, you have to install __docker-compose and docker__.

##### Usage

```bash
  gcl https://github.com/trobert42/inception.git
  cd inception
  make
```


## Project Overview:

### Summary:

Embark on a journey to enhance your system administration skills through the utilization of Docker virtualization. Inception challenges you to create a robust infrastructure composed of various services, all orchestrated within Docker containers running on your personal virtual machine.

### Key Features:

1. Virtualized Environment: Set up and configure a virtual machine environment to host Docker containers, enabling efficient management and deployment of services.
2. Docker Compose Mastery: Leverage Docker Compose to define and manage multi-container Docker applications, streamlining the setup and orchestration of complex infrastructures.
3. Service Modularization: Break down your infrastructure into distinct services, each running in its dedicated Docker container. Utilize Dockerfiles to customize and build Docker images for each service.
4. Security and Best Practices: Implement best practices for Dockerfile creation, emphasizing security and efficiency. Utilize environment variables and .env files to manage sensitive information securely.
5. Network Configuration: Establish a Docker network to facilitate communication between containers while adhering to security and performance standards. Ensure containers restart automatically in case of failure.
6. Container Orchestration: Explore PID 1 and daemon best practices to ensure proper container initialization and execution. Avoid hacky patches and adhere to Docker's recommended practices for running containers.

### Things to Do:

1. Virtual Machine Setup: Configure a virtual machine environment to serve as the host for your Docker containers, providing the necessary resources for seamless operation.
2. Dockerfile Creation: Write custom Dockerfiles for each service in your infrastructure, adhering to performance and security guidelines. Avoid using ready-made Docker images and pull requests, opting instead to build images from scratch.
3. Service Configuration: Set up essential services such as NGINX with TLSv1.2 or TLSv1.3, WordPress with php-fpm, and MariaDB in dedicated Docker containers. Configure volumes for database and website files, ensuring data persistence and availability.
4. Network and Security: Establish a Docker network to facilitate inter-container communication while enforcing security measures. Utilize environment variables and .env files to manage sensitive information securely.
5. Domain Configuration: Configure domain names to point to your local IP address, simplifying access to your services within the virtual environment. Implement TLS encryption for secure communication over port 443.
6. Bonus Challenges: Explore bonus tasks such as setting up Redis cache for WordPress, FTP server integration, creating a static website, deploying Adminer, or implementing a custom service of your choice to enhance your project further.

Dive deep into the realm of system administration with Inception, where you'll harness the power of Docker virtualization to build and manage a sophisticated infrastructure with precision and expertise.
