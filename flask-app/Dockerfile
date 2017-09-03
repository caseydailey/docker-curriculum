# Instructions copied from - https://hub.docker.com/_/python/
#'FROM' specifies our base image. since our application is written in python, the base image we're going to use is Python 3.
#'-onbuild' means that this image includes helpers that automate the boring parts of getting an app up and running. 
#the build will COPY a requirements.txt file RUN pip install on this and copy the current directory into usr/src/app

FROM python:3-onbuild

# tell the port number the container should expose
EXPOSE 5000

# run the command ``` python ./app.py ```
CMD ["python", "./app.py"]

# no we can run ```docker build``` 
