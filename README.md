# Docker - Personal Learning Notes

## Docker - Resources
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

## Docker Container


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

**Virtual Machines - e.g. VMware**
- Single physical server runs multiple virtual machines using Hypervisor
- Each single VM hosts a single application
- Each single VM is a slice of the server resources
- BAD: Operating System on each VM "steals" server resources (CPU, RAM, Disk)
- BAD: Operating System licenses are needed
- BAD: Each VM needs to be administrated

**Containers**
- Single physical server has a single operating system installed
- Operating system runs multiple containers
- Each single container is a slice of operating system
- Each single container runs a single application
