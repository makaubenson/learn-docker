# Docker
## What is Docker
- A platform for building, running and shipping applications in a consistent manner.
- Docker easily helps pacjage our application with everything it needs and run it anywhere in any machine.
### Why use docker?
- It makes development easier by providing an isolated environment to build your app without affecting the rest of your system or other apps on your computer.
- **Ease of deployment** - With the help of containers we can package up an entire app into one file that contains all its dependencies.
- It makes the development environment portable across machines (Windows/Linux)
- It provides an easy way to package your app so that anyone can download or build from source code without having to install dependencies on their own computer system
- Allows us to package an app alongside all of its dependencies into one image that can be deployed on any server without worrying about dependency conflicts.
- It allows us to package up an app or service into one container that can be deployed on any server without worrying about dependencies.

## Virtual Machines and Containers
- Container is an isolated environment for running and application.
- `VM` runs on top of host OS like Windows or Linux but `container` does not have access to underlying hardware resources(RAM etc). Basically its and abstraction of a machine.

### Problems with VM
- Each VM needs a full-blown OS
- Slow to start
- Resource intensive (CPU, MEMORY ETC)
- Limitations on number of VMs to run on a machine

### What of Containers
- Allow running multiple apps in isolation,
- ARe light weight
- Use OS of the Host
- start quickly
- Need less H/W Resources

## Docker Architecture
- Uses client-server achitecture , i.e it has a client component that talks to a server component(Docker Engine) using RESTFul API.  
- Docker Engine sits in the background and takes care of building and running docker conatiners. 
- In simple terms a Container is just a process, similar to other processes running on your computer. They dont have full-blown OS, it shares kernel of the Host. By this we mean, ON LInux Comp, we can only run Linux Containers and the same to other OS

## Development worflow
- Take app and dockerise it, just add a docker file(so that it can be run by docker)
## What is a docker file?
-  Docker file Plain text file that includes instructions that docker uses to package application to an image, the image contains everything our applications needs to run. Typically:
    - A cut-down os
    - A runtime environment e.g node
    - Application files
    - Third party libraries
    - Environment variables

- So we create a docker file, give it to docker for packaging our application into an image.
- Once we have the image, we tell docker to start a container using that image. 
- A container is just a process, however its a special type of process since it has it own file system provided by the application.
- So our application gets loaded inside a container and this is how we run it locally on our dev machine, `docker run ...` basi cally we tell docker to run it inside a container.

## Beauty of Docker
- Once we have the image we can push it to Registry such as `Docker Hub`, docker hub to docker is like github to git. Its a storage for docker images that anynone can use. Once our images are on docker hub, we can pull them to any machine running docker.

### To See all Images on a computer
-   `docker image ls`

## Managing Packages
- We use apt install <package name>

- `Remember` in linux, everything is a file, whether a processes, directories etc
