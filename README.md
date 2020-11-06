# Docker For Development

This project demonstrates some of the use cases of Docker for software development. The use cases are examples of how to run different kinds of applications in Docker containers and should be used with caution. The examples are not intended to be used for running production applications and are not secure. They are intended for learning purposes only.

## Instructions

Follow the instructions below for running each example.

### Python

From a Linux, MacOS, or Cygwin terminal, run `./python` from the python directory to launch the Python REPL. You can also use `./python my_script.py` to execute Python scripts. View the contents of the python file to see the docker command being executed.

### RabbitMQ

From a Linux, MacOS, or Cygwin terminal, run `./rabbitmq` from the rabbitmq directory to launch the Docker container "dev-rabbit". You can then access the RabbitMQ Management UI by navigating to http://localhost:15672. View the contents of the rabbitmq file to see the docker command being executed.

### Neo4j

First, in a Linux, MacOS, or Cygwin terminal, navigate to your home directory if you aren't already there. Create a new directory with the command `mkdir neoj4/data`. Next, run `./neo4j` from the neo4j directory to launch the Docker container "dev-ne04j". You can then access the Neo4j UI by navigating to http://localhost:7474. View the contents of the neo4j file to see the docker command being executed.

### Postgresql

First, in a Linux, MacOS, or Cygwin terminal, naviage to your home directory if you aren't already there. Create a new directory with the command `mkdir pgdata`. Next, run `./postgres` from the postgresql directory to run the postgresql database. Once postgres is running, you can connect to the postgres database from a Database Management tool such as pgAdmin. Alternatively, you can run psql in the container with the command `docker exec -it dev-postgres psql -U postgres`.

### MySQL

First, in a Linux, MacOS, or Cygwin terminal, navigate to your home directory if you aren't already there. Create a new directory with the command `mkdir mysql`. Next, run `./mysql` from the mysql directory to run the MySQL database. Once the container is running, you can connect to the MySQL database from a Database Management tool such as MySQL Workbench. Alternatively, you can run mysql in in the container with the command `docker exec -it dev-mysql mysql`.



### Go

First set the environment variables `GOOS` and `GOARCH` to match the operating system and CPU architecture of your machine. Next, run `./go` from the golang directory, followed by any command line arguments needed to use the go tool.

### Tesseract

First, create the tesseract_ocr Docker Image by running `docker build -t tesseract_ocr:latest .` in the tesseract directory. Next, run tesseract with any command line arguments with the command `./tesseract` in the tesseract directory.

