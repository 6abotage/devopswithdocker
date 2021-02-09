FROM ubuntu:16.04
RUN apt-get update && apt-get -y install curl
WORKDIR /mydir
COPY test.sh .
CMD ["/mydir/test.sh"]