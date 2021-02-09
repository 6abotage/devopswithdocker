FROM ubuntu:16.04

WORKDIR /mydir 
# WORKDIR will create and set the current working directory to /mydir after this directive
RUN apt-get update && apt-get install -y wget 
RUN touch hello.txt
# will execute  command with /bin/sh -c prefix 
# because of WORKDIR => same as RUN touch /mydir/hello.txt
RUN  touch local.txt
COPY local.txt .
# copes an existing local file to the second argument
RUN wget http://example.com/index.html
CMD ["/bin/bash"]
# cmd is the command that will be executed when using docker container run
# any dockerfile should have exactly one CMD instruction 
# if more than one, only the last one will be executed