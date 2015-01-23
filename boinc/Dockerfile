FROM phusion/baseimage:0.9.15
MAINTAINER trurl rick.hughes@pobox.com
ENV DEBIAN_FRONTEND noninteractive

RUN apt-get update
RUN apt-get install -qy boinc-client

VOLUME /var/lib/boinc-client

EXPOSE 31416

USER boinc
WORKDIR /var/lib/boinc-client

ENTRYPOINT ["boinc","--allow_remote_gui_rpc"]
