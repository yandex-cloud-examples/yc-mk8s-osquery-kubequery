FROM ubuntu:20.04

WORKDIR /osquery

RUN apt-get update \
  && apt-get install -y software-properties-common \
  && apt-get install apt-transport-https

RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 1484120AC4E9F8A1A577AEEE97A80C63C9D8B80B \
&& add-apt-repository 'deb [arch=amd64] https://pkg.osquery.io/deb deb main' \
&& apt-get update \
&& apt-get install osquery


