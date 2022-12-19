# container-from-scratch-python
This is building a container from scratch

## Build the Container Yourself and Push to Docker Hub

### Build image
*(If you want to develop yourself)* 
docker build --tag=hello-ck .

### List docker images
docker image ls

### Run my newly built container

docker run -it hello-ck python app.py --name "cameronkenn"

### Push to Docker Hub

*Note:  You will need to change for your Docker Hub Repo*
docker push camkennington/container:tagname

## Run it yourself


```

## Pass in a command

```bash
docker run -it hello-ck python app.py --name "cameronkenn"
#the output
Hello cameronkenn!
```

## Push to Amazon ECR

1.  Create ECR repository


### More things Do

* Lint the code with Github Actions (see the Makefile)
* Automatically build the container after lint, and push to DockerHub or some other Container Registery
