FROM ubuntu:latest
RUN apt-get update -y
RUN apt-get install -y python-pip python-dev build-essential wget
COPY . /app
WORKDIR /app
RUN chmod -R g+rx,o+rx /app
RUN pip install -r requirements.txt
ENTRYPOINT ["python"]
CMD ["app.py"]
