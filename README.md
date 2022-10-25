# *Assignment 1*

**Specification**

Develop one API endpoint that accepts a GET call without parameters and returns a text “Hello, world!” message.
The HTTP handler should be developed in C#, Dockerized, and deployed to the target location through an automated CI/CD pipeline.

**Steps**

1. Create a Git repository and upload to it a README file with the Assignment description
2. Develop the HTTP handler locally and upload the Git repository
3. Dockerize it so that anybody who can get the code can run it locally on his machine via a local “docker-compose up” command
4. Decide in which GCP environment to deploy (CloudRun or GKE)
5. Develop a CI/CD pipeline (TeamCity or Jenkins) to automatically deploy the code on the target platform


### How to build and execute the app
- Clone the repository and navigate to the folder in the terminal
- Execute the following command
    ```Powershell
            docker compose up
    ```
- The app will now be accessible on [`http://localhost:8000`](http://localhost:8000)
- To close the app execute the following command in a terminal
    ```Powershell
            docker compose down
    ```