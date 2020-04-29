FROM ubuntu:latest


USER root
RUN apt-get update -qq \
&& apt-get install -qqy python3-pip vim git
RUN pip freeze > requirements.txt && mkdir workspace
