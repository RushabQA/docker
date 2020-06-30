#Use Python Image
FROM python:latest

# Install apt dependencies
RUN apt-get update && apt-get install -y python3-pip

# Copy contents into image
COPY . .

# run pip dependencies
RUN pip3 install flask 
RUN pip3 install flask-sqlalchemy
RUN pip3 install pymysql

# Expose correct port
EXPOSE 5000

# Create an entrypoint
ENTRYPOINT [ "/usr/local/bin/python3", "app.py" ]



