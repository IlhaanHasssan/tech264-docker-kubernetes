# ***DOCKER COMPOSE***
- [***DOCKER COMPOSE***](#docker-compose)
  - [***Why use it?***](#why-use-it)
  - [***How to use it:***](#how-to-use-it)
    - [***What do you need to install for it to work?***](#what-do-you-need-to-install-for-it-to-work)
    - [***How to store your docker compose file?***](#how-to-store-your-docker-compose-file)
    - [***Find out about these docker compose commands to:***](#find-out-about-these-docker-compose-commands-to)
      - [***Manage your application***](#manage-your-application)
      - [***Start the application (without detached mode)***](#start-the-application-without-detached-mode)
      - [***Start the application (in detached mode)***](#start-the-application-in-detached-mode)
      - [***What is the difference between running your application with or without detached mode***](#what-is-the-difference-between-running-your-application-with-or-without-detached-mode)
      - [***Stop the application***](#stop-the-application)
    - [***Check services running with docker compose***](#check-services-running-with-docker-compose)
    - [***View logs in real-time***](#view-logs-in-real-time)
    - [***View docker compose images***](#view-docker-compose-images)
 
## ***Why use it?***
- **Simplicity**: It allows you to configure multiple serves in a signle `docker-compose.yaml` file, making it easy to orchestrate containers in a structured and reproducible way.
 
- **Environment Consistency**: Ensures all dependencies and configurations are replicable in a development, testing and production environment.
 
## ***How to use it:***
1. Define your application's services, networks and volumes in a `docker-compose.yaml` file.
2. Use `docker-compose` commands to **build**, **start**, **stop** and **manage** these services.
 
### ***What do you need to install for it to work?***
- Docker Compose, which is included if you have downloaded **`Docker Desktop`**.
 
### ***How to store your docker compose file?***
- Store **`docker-compose.yaml`** in the root directory of your project for easy access and version control.
 
### ***Find out about these docker compose commands to:***
 
#### ***Manage your application***
- **`docker-compose up`**: Builds, (re)creates, and starts containers as defined in docker-compose.yml.
- **`docker-compose down`**: Stops and removes containers, networks, and volumes created by up.
 
#### ***Start the application (without detached mode)***
- **`docker-compose up`**: Runs services and outputs logs to the console.
 
#### ***Start the application (in detached mode)***
- **`docker-compose up -d`**: Runs services in the background.
 
#### ***What is the difference between running your application with or without detached mode***
- **Detached Mode (-d)**: Runs containers in the background, allowing you to use the terminal for other commands.
- **Non-Detached Mode**: Runs containers in the foreground, displaying logs and keeping the terminal focused on the running services.
 
#### ***Stop the application***
- **`docker-compose stop`**: Stops running containers but keeps the containers and network in place.
 
### ***Check services running with docker compose***
- **`docker-compose ps`**: Lists all services defined in 
- **`docker-compose.yaml`** and shows their status.
 
### ***View logs in real-time***
**`docker-compose logs -f`**: Shows live logs for all services. 
- Use **`-f`** (follow) to update logs in real-time.
 
### ***View docker compose images***
- **`docker-compose images`**: Lists images used by your Docker Compose services.