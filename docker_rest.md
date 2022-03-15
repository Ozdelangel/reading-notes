# How to get Docker

1. remember you need to get the desktop app an make a free account
2. when docker is done installing we can confirm correct version is running it should be at least version 19 and you can check this by using `docker --version`e
3. Docker Compose is an additional tool that is automatically included with Windows downloads of Docker
4. if you are on Linux you have to add it manually using `sudo pip install docker_compose`
## to confirm docker is installed
1. We have to run our first command `docker run hello-world`
2. a good command to inspect Docker is `docker info`
it comes with a lot of stuff but focus on the top line
3. it will show the hello-world  image which we just downloaded. How about inspecting, containers running, paused, or stopped
## Dockerized Django
1. create a dockerfile for our image which completely replace our local env, so this will have python 3 and django then we have to add our docker-compose.yml file for the container instructions. Make each file via the command line.
- touch `Dockerfile`
- touch `docker-compose.yml`

2. this `Dockerfile` has several commands run, copy, and add each create a new layer.

3. order matter in Dockerfiles since they are executed fro top-to-bottom. 