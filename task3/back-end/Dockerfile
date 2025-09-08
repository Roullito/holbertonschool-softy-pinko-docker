FROM ubuntu:latest
WORKDIR /app
RUN apt-get update && apt-get upgrade -y && apt-get install -y python3 python3-pip
RUN rm -f /usr/lib/python*/EXTERNALLY-MANAGED && pip3 install flask flask-cors
COPY api.py /app/api.py
CMD ["python3", "api.py"]
