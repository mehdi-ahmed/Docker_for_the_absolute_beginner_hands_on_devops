FROM ubuntu:latest

# install flask server
RUN apt-get update -y
RUN apt-get install -y python-pip python-dev build-essential
RUN pip install flask
RUN pip install flask-mysql


COPY . /opt/source-code

ENTRYPOINT FLASK_APP=/opt/source-code/app.py flask run