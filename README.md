# docker
Sample of project with Docker


-----------------

## docker hub

[samples of dockerfiles](https://hub.docker.com/search?type=image)

-----------------

## docker tutorial

[link](https://www.docker.com/101-tutorial)


-----------------

## install docker Ubuntu

[link](https://www.digitalocean.com/community/tutorials/how-to-install-and-use-docker-on-ubuntu-20-04-ru)

``` 
sudo apt update
sudo apt install apt-transport-https ca-certificates curl software-properties-common
curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo apt-key add -
sudo add-apt-repository "deb [arch=amd64] https://download.docker.com/linux/ubuntu focal stable"
sudo apt update
apt-cache policy docker-ce

sudo apt install docker-ce

sudo systemctl status docker

sudo docker run hello-world
```

## get docker

[link](https://docs.docker.com/get-docker/)

[link](https://docs.docker.com/engine/install/ubuntu/)

```
sudo apt-get update
sudo apt install curl
sudo apt-get install \
    apt-transport-https \
    ca-certificates \
    gnupg-agent \
    software-properties-common
    
curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo apt-key add -

sudo add-apt-repository \
   "deb [arch=amd64] https://download.docker.com/linux/ubuntu \
   $(lsb_release -cs) \
   stable"
   
sudo apt-get update
sudo apt-get install docker-ce docker-ce-cli containerd.io

apt-cache madison docker-ce

sudo apt-get install docker-ce=<VERSION_STRING> docker-ce-cli=<VERSION_STRING> containerd.io
sudo apt-get install docker-ce containerd.io

sudo docker run hello-world

```

-----------------



-----------------



-----------------


