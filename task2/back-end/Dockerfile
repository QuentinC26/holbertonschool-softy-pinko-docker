FROM ubuntu:latest
WORKDIR /app
RUN apt-get update -y && apt-get upgrade -y
RUN apt-get update -y && apt-get upgrade python3 -y
RUN apt-get update -y && apt-get upgrade python3-pip -y
RUN rm /usr/lib/python*/EXTERNALLY-MANAGED
RUN pip3 install Flask
COPY api.py /app
CMD ["python3", "api.py"]
