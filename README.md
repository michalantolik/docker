# Docker - Personal Learning Notes

## Docker - Resources
- https://www.docker.com/
- https://docs.docker.com/
- https://learn.microsoft.com/en-us/virtualization/windowscontainers/
- https://www.linkedin.com/learning/docker-for-windows/

## Docker is an open source platform for container management
- **Docker Desktop** - Community Edition (CE)
  - Free
  - Windows and Mac
- **Docker Enterprise** - Enterprise Edition (EE)
  - Paid
  - Windows and Linux
  
## Docker - History
- March 2013 - Solomon Hykes introduced Docker at PyCon tech talk
- June 2014 - Docker Engine 1.0 made general availability (GA) at DockerCon 1
- April 2018 - Docker Enterprise Edition 2.0

## Docker Engine
- Engine for both Docker CE and Docker EE

## Docker Hub
- **Registry of Docker container images** (public and private) ...
- ... a kind of marketplace 

## Docker Desktop
- It's just a **Windows version of Docker Desktop** (CE) ...
- ... designed to run on Windows 10 or newer
- ... provides friendly enviornment for building, shipping and running Docker containers

## Docker Desktop - What is included
- Docker Engine
- Docker CLI client
- Docker Compose
- Docker Machine
- Kitematic

## Docker Image VS Docker Container
- **Docker Image** is an executable packaged application
- **Docker Container** is a running instance of an image

## Docker Container - Benefits
- **Flexible** --> any application (Windows/Linux) no matter how complex, can be containerized
- **Lightweight** -->
- **Interchangeable** --> can easily be updated or replaced as needed
- **Portable** --> can easily be moved from local laptop to data center and then to the cloud
- **Scalable** --> can easily be added/removed as your demands increases/decreases
- **Stackable** --> can create hierarchical stacks of containers with interrelated service and shared dependencies

## Container VS Virtual Machine - Simply
- **Virtual Machine** virtualizes physical server resources (hardware) --> and builds virtual machines
- **Container** virtualizes operating system --> separate virtual OS for each container

## Container VS Virtual Machine - In depth
**Single physical server**
- Single physical server hosts a single application
- BAD: Often overpowered servers were bought

**Virtual Machines - e.g. VMware, Microsoft Hyper-V**
- Single physical server runs multiple virtual machines using Hypervisor
- Each single VM hosts a single application
- Each single VM is a slice of the server resources
- BAD: Operating System on each VM "steals" server resources (CPU, RAM, Disk)
- BAD: Operating System licenses are needed
- BAD: Hypervisor license is needed
- BAD: Each VM needs to be administrated
- BAD: Large in size
- BAD: Slow boot
- GOOD: Can run traditional applications (not containerized...)

**Containers**
- Single physical server has a single operating system installed
- Operating system runs multiple containers
- Each single container is a slice of operating system
- Each single container runs a single application

## Docker Desktop - Installation
- Make sure that your computer OS allows you to run Docker for Windows
- Enable BIOS level hardware virtualization in BIOS settings
- Download Docker Desktop from website and install or run `choco install docker-desktop`
- Restart PC and run Docker Desktop
- Install WSL 2 Linux kernel if prompted *(Windows Subsystem for Linux)*
  - https://learn.microsoft.com/en-us/windows/wsl/install-manual#step-4---download-the-linux-kernel-update-package
- Restart Docker Desktop if prompted
- Login with Docker ID
- See https://docs.docker.com/

## Kubernetes

**Kubernetes - History**
- Around 1999 Google was already running their services in containers (search engine, gmail)
- Google created Borg -> Omega -> Kubernetes (open source)
- "Kubernetes" means "Helmsman" in Greek

**Docker VS Kubernetes**
- Docker cares about low-level stuff: start/stop/delete containers
- Kubernetes cares about high-level stuff: schedule/scale/heal/update ...
- ... **it is an orchestration tool**
- ... it orchestrates nodes and tells Container Runtime (Docker instance) when to start/stop/delete containers

**Kubernetes - Node**
- Container Runtime
- Kubernetes Agent

## Docker - Basic commands
```bash
# Show help

docker
```
