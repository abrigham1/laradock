FROM phusion/baseimage:latest

LABEL maintainer="Mahmoud Zalt <mahmoud@zalt.me>"

COPY ./laradock/certbot/run-certbot.sh /root/certbot/run-certbot.sh

COPY ./laradock/certbot/letsencrypt/ /var/www/letsencrypt

RUN apt-get update
RUN apt-get install -y letsencrypt

ENTRYPOINT bash -c "bash /root/certbot/run-certbot.sh && sleep infinity"
