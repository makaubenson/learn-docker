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


  