FROM continuumio/anaconda3
LABEL maintainer="Aaron Brigham"

ARG INSTALL_FLASK=false

RUN if [ ${INSTALL_FLASK} = true ]; then \
    pip install Flask
;fi

WORKDIR /var/www