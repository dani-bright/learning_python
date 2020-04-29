FROM ubuntu:latest


USER root
RUN apt-get update -qq \
&& apt-get install -qqy python3-pip vim git
RUN mkdir workspace && pip3 freeze > requirements.txt && pip3 install jupyter
RUN cd workspace && git clone --verbose https://github.com/dbebli/learning_python.git \
&& cd learning_python
CMD ["jupyter", "notebook", "--port=8888", "--no-browser", "--ip=0.0.0.0", "--allow-root"]