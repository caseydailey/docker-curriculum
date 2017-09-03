# Instructions copied from - https://hub.docker.com/_/python/
#'FROM' specifies our base image. since our application is written in python, the base image we're going to use is Python 3.
#'-onbuild' means that this image includes helpers that automate the boring parts of getting an app up and running. 
#the build will COPY a requirements.txt file RUN pip install on this and copy the current directory into usr/src/app

FROM python:3-onbuild

# tell the port number the container should expose
EXPOSE 5000

# run the command ``` python ./app.py ```
CMD ["python", "./app.py"]

########################################

#that's it.

# no we can run ```docker build -t caseydailey/catnip .``` 
# the '-t' is an optional tag name flag and the '.' 
#tell is where the 'Dockerfile' is (current context in this case)

# then ``` docker run -p 8888:5000 caseydailey/catnip  ```
# '-p' is exposes the port inside the container (5000) 
#externally through 8888

# next we push it up to Dockerhub with :
# ``` docker push caseydailey/catnip ```
# now anyone with docker installed can pull this down and run it with:

# ``` docker run -p 8888:5000 caseydailey/catnip ```




