FROM debian:latest
MAINTAINER saji hassanzadeh.sd@gmail.com
RUN apt-get update -y && \
    apt-get install -y python-pip \
    python-dev
ADD . /app
WORKDIR /app
RUN pip install -r requirements.txt
EXPOSE 5000
ENTRYPOINT ["python"]
CMD ["webapp.py"]

