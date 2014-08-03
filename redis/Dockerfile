FROM ubuntu:14.04
MAINTAINER Dinesh Weerapurage "xydinesh@gmail.com"
# set an environment variable with ENV
ENV REFRESHED_AT 2014-08-03
RUN apt-get -qq update

RUN apt-get install -y busybox dropbear net-tools wget emacs redis-server
RUN apt-get clean
RUN mkdir -p /root/.ssh

# storage port, JMX, Thrift, CQL Native
EXPOSE 6379

CMD ["redis-server"]
