# lfd
letsencrypt with anaconda flask in a dockercontainer


# TODO replace:
# IP, 
# pem file
# env for letsencrypt
# start amazon instance
# connect to amazon instance:
ssh -i JaapOosterbroek_EC2_EUC1_2.pem ubuntu@35.158.141.122

# get repro and build docker
sudo apt-get update
sudo apt-get install docker.io
git clone https://github.com/kozzion/lfd.git
cd ~/lfd
sudo docker pull continuumio/anaconda3
sudo docker build -t relay.
sudo docker run -p 443:443 -it relay

sudo docker run -p 80:80 -e PYTHON_ENV='DEBUG' relay




#inside container

sudo apt-get install letsencrypt




--usefull docker commands

docker --version
sudo docker image ls
sudo docker container ls

sudo docker rm -f $(sudo docker ps -a -q)  Kill all dockers
sudo docker rmi -f $(sudo docker images -q) Remove all images
sudo docker container stop [d87d91196ed9]

sudo docker run -p 80:80 -it relay

//Reload eviroment after installing anaconda
source ~/.bashrc  
//Top sorted by mem
top -o %MEM


-- for copying data
use winscp
killall5 -9
