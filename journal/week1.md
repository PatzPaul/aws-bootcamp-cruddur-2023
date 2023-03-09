# Week 1 — App Containerization

This week went through entire checklist and got to install docker and containerize our application parts also added some database services, Here are a few things that were performed.

## Setting up Dockerfile for the frontend and Backend
This involved making a dockerfile for our platform backend which based off requirements.txt file to load the necessary flask components and then proceeded to build and spin up the backend container on port 4567 
where the -t tag is used ffor naming purposes and the --rm tag.
Dockerfile was made for front end and respective code added following the relevant steps and then finally tried to run each conatiner dockerfile as an external script with the following command after some sorting the ordering of the syntax

```
docker run --rm -p 4567:4567 -it -e FRONTEND_URL ='*' -e BACKEND_URL = '*' backend-flask

```
## Adding a docker compose file on our project root directory 
Docker compose file is set up in the project root directory to run both containers.Relevant code was added as per instructions for both containers and i also learned a thing or two when it comes to debugging environment variables.

## finished watching pricing and security video
This was folowed up by tyhe container security considerations where i got introduced to some best security practices like scanning images for any secrets or risky data that may not be necessariry needed before pushing the container.Tried implementing some of the best practises from the video on our dockerfile

## created a notification feature by editing front end and backend
Added some backend configuration for notifications page where i learned about openapi and how to key in the neccessary api endpoint for our respective notification page to communicate with and receive dummy data 
After writing the flask backend endpoint for the notifications page, went on to create and write a notifications page on the react frontend and after some api configuration final checks was able to get the notifications page with minimal stress when following the instructions.

## installation of postgres and dynamodb
Got to learn the handling of dynamodb and postgres as services and how to declare them in our project. An interesting point i got was how the driver local is targeted for our dynamodb local and as per the instructors explanation got to understand the installation of postgres for our project in accordance with the respective ports.

## run dynamodb local and postgres after installation 
tried creating a new postgres table after installing the database variable extension from the marketplace and went on to test some postgres commands such as listing created tables.

# Extra things considered in the homework
Extra work to finalise the week focuses on configuration of ports to stay public for our different services in the docker workspace and also implementing a healthcheck for our docker compose file version 
