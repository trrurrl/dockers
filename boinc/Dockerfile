FROM phusion/baseimage:0.9.15
MAINTAINER trurl rick.hughes@pobox.com

RUN apt-get update
RUN DEBIAN_FRONTEND=noninteractive apt-get install -y boinc-client
#RUN mkdir /var/lib/boinc-client/slots

USER boinc
WORKDIR /var/lib/boinc-client
ENTRYPOINT ["boinc"]
