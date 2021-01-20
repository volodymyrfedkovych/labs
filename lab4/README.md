1. Read about Docker
***
2. Check Docker install by command `sudo docker -v` `sudo docker -h` `sudo docker run docker/whalesay cowsay Docker is fun and redirect to my_work.log`
***
3. Read Docker documentation
***
4. Create image w/ Django site which site create in previous lab by this commands: docker pull python:3.8-slim docker images docker inspect python:3.8-slim
***
5. [Link](https://hub.docker.com/repository/docker/volodymyrfedkovych/lab4) repo Docker 
***
6. sudo docker build -t volodymyrfedkovych:django . sudo docker push volodymyfedkovych/lab4:django
***
7. Run docker image sudo docker run -it --net=host --rm -p 8000:8000 volodymyfedkovych/lab4:django
***
8. Build Dockerfile.site image sudo docker build -f Dockerfile.site -t volodymyfedkovych/lab4:monitoring . and push it to Docker sudo docker push volodymyfedkovych/lab4:monitoring
***
Run both containers sudo docker run -it --net=host --rm -p 8000:8000 volodymyfedkovych/lab4:django sudo docker run -it --net=host -v $(pwd)/logs:/app/logs volodymyfedkovych/lab4:monitoring 
***
**Update READMEFILE and create pull request**
***
