FROM ubuntu:latest
MAINTAINER Flevian Kanaiza "fleviankanaiza@live.com"
RUN apt-get update -y
RUN apt-get install -y  python-pip python-dev build-essential apt-utils
RUN pip install --upgrade pip
COPY . /app
WORKDIR /app
RUN pip install -r requirements.txt
ENTRYPOINT ["python"]
CMD ["app.py"]