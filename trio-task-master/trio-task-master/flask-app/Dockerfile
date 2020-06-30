#Use Python Image

FROM python:3.8

# Install apt dependencies
 
RUN apt update

RUN apt install python3-pip -y
# Copy contents into image
 
COPY . . 

# run pip dependencies

RUN pip3 install flask
RUN pip3 install flask_sqlalchemy
RUN pip3 install pymysql
# Expose correct port

EXPOSE 5000

# Create an entrypoint

ENTRYPOINT ["/usr/local/bin/python3", "app.py"]
