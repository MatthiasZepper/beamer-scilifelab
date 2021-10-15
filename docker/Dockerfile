
## Contributed by Walter Schulze (@awalterschulze)
## Simplified by Dirk Eddelbuettel (@eddelbuettel)

FROM ubuntu:focal
ENV DEBIAN_FRONTEND noninteractive

RUN apt-get update -q
## Lato is designed by Łukasz Dziedzic
## Biolinum is the Sans-Serif Font from the Libertine Package, designed by Philipp H. Poll
RUN apt-get install -qy texlive-full fonts-lato fonts-linuxlibertine
RUN apt-get install -qy \
    gnuplot \
    wget \
    build-essential

WORKDIR /data
VOLUME ["/data"]
