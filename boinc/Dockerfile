FROM phusion/baseimage:0.9.15
MAINTAINER trurl rick.hughes@pobox.com
ENV DEBIAN_FRONTEND noninteractive

RUN apt-get update
RUN apt-get install -qy boinc-client

VOLUME /var/lib/boinc-client

EXPOSE 31416

USER boinc
WORKDIR /var/lib/boinc-client

RUN echo "" > /var/lib/boinc-client/gui_rpc_auth.cfg

ENTRYPOINT ["boinc","allow_remote_gui_rpc"]
