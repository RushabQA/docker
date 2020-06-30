# Derived from official mysql image (our base image)
FROM mysql:latest

# Add a database
ENV MYSQL_DATABSE=flask.db

COPY ./CreateTable.sql docker-entrypoint-initdb.d/


# Add the content of the .sql file to your image
# All scripts in docker-entrypoint-initdb.d/ are automatically
# executed during container startup
