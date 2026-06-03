
apt = linux package manger
apt update = update package list
apt list = show packages in apt database
apt search nano(package name) = search for the package name in list of the repository
apt install nano(package name)= install the package
apt remove nano(package name)= removes the package

if you confront an error while installing an package, update the apt and then try to install thee package.

image like a .exe file for installing of an application and containers are those applications, every time we run `docker run imagename`, we create a container, by closing the terminal container doesn't get removed unless we do it explicitly, for checking list of your containers type
`docker ps -a`, we can give each of these application or container to have the specific container with its own unique packages and files, because when we install package on a container (packages are liked saved file in a game or application which game or application represents the docker container ), it only get installed on that particular container not the other ones, when you run an image with size of 70 mb and you have run that image in 4 containers, it still occupies 70 mb and each container only occupies amount of size the packages and each file in it has.

for naming our container so we can run the same certain container we use command below:

`docker run -it --name myubuntu (container name) ubuntu:jammy (image name)`
use command below when you're creating your container

`docker start -ai myubuntu`
use command above for starting the specific container

