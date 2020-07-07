# react-start-docker
React App Start with Semantic UI &amp; GitHub Pages &amp; Dockerfile

[DEMO at vercel.com](https://react-go.now.sh/)

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


 