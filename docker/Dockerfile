FROM ubuntu:latest


USER root
RUN apt-get update -qq \
&& apt-get install -qqy python3-pip vim git
RUN mkdir workspace && pip3 freeze > requirements.txt 
