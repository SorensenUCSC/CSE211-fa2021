---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

title: "Docker Setup"
layout: single
classes: wide
---

This guide walks you through developing and running your assignments using a Docker container running Ubuntu.

## Install Docker
Follow instructions [here](https://docs.docker.com/get-docker/).

## Create a volume
Docker containers do not persist their data when closed. Therefore, we need to create a volume so that any modifications we make in the container will persist across restarts. To create the volume used in this course's official image, run the following command:

`docker volume create assignments`

## Download and run the container
Run the following commands:

```
docker pull sorensenucsc/cse211-fa2021:latest
docker run -v assignments:/assignments -it sorensenucsc/cse211-fa2021:latest
```

While the details of running docker containers are unnecessary for this course, it might be helpful to understand what each part of the above command is doing.
- `docker pull` downloads the specified container, which in this case is `sorensenucsc/cse211-fa2021:latest`, where `sorensenucsc/cse211-fa2021` is the image name and `latest` is the tag. Docker allows multiple tags for the same image, but for this course we will most likely only be using the default `latest` tag for images.
- `docker run` runs the specified container, which we just pulled above.
- `-v` mounts a volume from the host (your computer) to the docker container. We are mounting the volume we created in the step above to the directory `/assignments` inside the container.
- `-it` gives us an interactive, terminal based session. Without this, the container would immediately exit.

Make sure that you regularly pull before running. We'll be updating the container as the class goes on and pulling ensures you'll have the most up-to-date environment when developing.

## Develop inside the container
You'll notice that the container places you in the `/assignments` directory when started. Any data saved in this directory or any of its subdirectories will persist when you exit the container. Note that data placed in any other directory will not be persisted, so make sure you're in the right place when writing your code!

Homework material will either be available to download using `wget`, or pushed into a data directory of this docker image. Look for instructions on how to do this when the homework is released. 

The container supports vim and emacs by default, but please let me know if you'd like us to install any other text editors. Additionally, git is installed if you want to keep your work under source control.

## Getting code out of the container
While running your container, use another terminal session and find the id of the container by running `docker ps`. Copy either the container id or the name, and run `docker cp <container-id>:/assignments/<path_to_code> .`. This will copy the file (or directory), to the current directory on your machine.

Another option, if you are using git, is to push your code to a remote repository such as GitHub or GitLab.

## Acknowledgements 

Thanks to Reese Levine and Gan Shen for the first iteration of this document for CSE 113 spring of 2021!
