# Tutorial: Containerize a .NET Core app

https://docs.microsoft.com/en-us/dotnet/core/docker/build-container

# Commands

// Create the image
docker build -t myimage -f Dockerfile .

//Create container from the image
docker create myimage

//List images
docker images

//List containers
docker ps -a

//Start container
docker start <container name>

//Stop Container
docker stop <container name>
  
//Delete container -  First Stop it
docker rm <container name>

//Delete images
docker rmi <image name> // Example. myimage:latest or mcr.microsoft.com/dotnet/core/aspnet:3.1
