# docker_nginx_basic_static
A very basic static site with Dockerfile to be run using nginx.

Most walkthroughs for running a static website in Docker are quite complicated. This is designed to be as simple/ basic as possible.

## Steps:
1. Input path to root directory in Dockerfile replacing /Users/jimsmith/Documents/docker-test-site/. The easiest way to do this in a mac is to drag and drop directory from Finder to Terminal to show this, then copy and paste into Dockerfile.

2. Build new image:
    
    (from root directory in CLI)

        $ docker build -t image_name .

    Use the following to check images:

        $ docker images

3. To run on port 80 (http://localhost:80):

        $ docker run -d -p 80:80 image_name

4. To stop:

        $ docker stop container_ID

    To find container_ID:

        $ docker ps
