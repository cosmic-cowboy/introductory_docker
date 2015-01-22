# Format : From repository[:version]
FROM	centos:centos6

# Format : MAINTAINER Name 
MAINTAINER hiro 

# repository
RUN yum -y update; yum clean all
RUN yum -y install epel-release; yum clean all

# Installation
# Import MongoDB 
RUN yum -y install mongodb-server; yum clean all

# Create the MongoDB data directory
RUN mkdir -p /data/db

# Expose port 27017 from the container to the host
EXPOSE 27017

# Set usr/bin/mongod as the dockerized entry-point application
ENTRYPOINT ["/usr/bin/mongod"]




