FROM phusion/baseimage:0.9.15
MAINTAINER trurl rick.hughes@pobox.com

RUN apt-get update
RUN DEBIAN_FRONTEND=noninteractive apt-get install -y boinc-client

USER boinc
WORKDIR /var/lib/boinc-client

ADD remote_hosts.cfg /var/lib/boinc-client/remote_hosts.cfg
ADD gui_rpc_auth.cfg /var/lib/boinc-client/gui_rpc_auth.cfg

ENTRYPOINT ["boinc"]
