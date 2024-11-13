FROM ubuntu:22.04

RUN apt update && apt install git -y && apt install apache2 -y

WORKDIR /tmp

COPY . .

ENV app=team hello=kaizen

EXPOSE 80

CMD ["apache2ctl", "-D", "FOREGROUND"]