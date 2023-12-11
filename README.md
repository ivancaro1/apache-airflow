# Installing Apache Airflow

## Hello there! 👋
It's time to install Apache Airflow, and you'll find that the process is straightforward.

## Prerequisites

First, ensure that you have Docker Desktop and Visual Studio Code installed. If not, check out the following links:

1. [Get Docker](https://docs.docker.com/get-docker/)
2. [Get Visual Studio Code](https://code.visualstudio.com/)

Docker requires privileged rights to function, so make sure you have the necessary permissions.

If you encounter any difficulties installing these tools, refer to the following helpful videos:

- [Install Docker on Windows 10](https://www.youtube.com/watch?v=1MgF3iINkjI)
- [Install Docker on Windows 10 with WSL 2](https://www.youtube.com/watch?v=UJbc5lJpaMQ)
- [Install Docker on Windows 11](https://www.youtube.com/watch?v=1MgF3iINkjI) *(Note: Link may be the same as for Windows 10)*

## Install Apache Airflow with Docker

1. Create a folder named `materials` in your `Documents` directory.

2. Download the [docker compose file](materials/docker-compose.yaml) into the `materials` folder.

3. If you right-click on the file and save it, you'll end up with `docker-compose.yaml.txt`. Remove the `.txt` extension, keeping it as `docker-compose.yaml`.

4. Open your terminal or CMD and navigate to `Documents/materials`.

5. Right-click below `docker-compose.yml` and create a new file named `.env` (ensure the dot is before `env`).

6. In the `.env` file, add the following lines:

    ```env
    AIRFLOW_IMAGE_NAME=apache/airflow:2.4.2
    AIRFLOW_UID=50000
    ```

    Save the file.

7. In your new terminal at the bottom of Visual Studio Code, type the command `docker-compose up -d` and press ENTER.

8. Open your web browser and go to `localhost:8080`.
