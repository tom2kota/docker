# react-start-docker
React App Start with Semantic UI &amp; GitHub Pages &amp; Dockerfile

[DEMO at vercel.com](https://react-go.now.sh/)

-----

## [Install Docker Toolbox on Windows](https://docs.docker.com/toolbox/toolbox_install_windows/)

Docker Toolbox provides a way to use Docker on Windows systems that do not meet minimal system requirements 
for the Docker Desktop for Windows app.

-----

## [Install Docker Desktop on Windows Home](https://docs.docker.com/docker-for-windows/install-windows-home/)

One of the advantages of the newer Docker Desktop for Windows solution is that it uses native virtualization 
and does not require VirtualBox to run Docker.

[Download from Docker Hub](https://hub.docker.com/editions/community/docker-ce-desktop-windows/)

###### System Requirements:
- Install Windows 10, version 1903 or higher.
- Enable the WSL 2 feature on Windows. For detailed instructions, refer to the [Microsoft documentation](https://docs.microsoft.com/en-us/windows/wsl/install-win10).
- The following hardware prerequisites are required to successfully run WSL 2 on Windows 10 Home:
    - 64 bit processor with Second Level Address Translation (SLAT)
    - 4GB system RAM
    - BIOS-level hardware virtualization support must be enabled in the BIOS settings. For more information, see [Virtualization](https://docs.docker.com/docker-for-windows/troubleshoot/#virtualization-must-be-enabled).
- Download and install the [Linux kernel update package](https://docs.microsoft.com/ru-ru/windows/wsl/wsl2-kernel).

-----


-----

#### Dockerfile:

```
FROM node:carbon

WORKDIR /usr/src/react-start

COPY ./ ./

RUN npm i

CMD ["/bin/bash"]
```

#### Run Docker
``` 
sudo docker build -t reactstart .

sudo docker run -it -p 3000:3000 reactstart
sudo docker run -it -d -p 3000:3000 reactstart

sudo docker ps
pwd && ls
```

#### Run project
``` 
npm start
```

#### Finish
``` 
CTRL + C

exit

sudo docker ps
sudo docker stop <CONTAINER ID>
```

-----


