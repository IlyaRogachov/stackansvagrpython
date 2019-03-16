FROM ubuntu:latest
RUN apt-get update -y
RUN apt-get install -y python-pip python-dev build-essential
RUN apt-get install -y python-mysqldb
COPY . /app
WORKDIR /app/main
RUN pip install flask_sqlalchemy
RUN pip install wheel
RUN pip install flask
RUN pip install pymysql
#CMD exec /bin/bash -c "trap : TERM INT; sleep infinity & wait"
EXPOSE 8080
CMD ["python", "main.py"]
