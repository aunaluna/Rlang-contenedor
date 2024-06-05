FROM r-base:4.3.3

RUN apt-get update && apt-get install -y \
    sudo \
    libcurl4-openssl-dev \
    libssl-dev \
    libxml2-dev

USER root

RUN R -e "install.packages('languageserver')"

WORKDIR /proyecto

COPY . /proyecto