FROM ubuntu:22.04
ENV DEBIAN_FRONTEND=noninteractive
RUN apt-get update && apt-get install -y --no-install-recommends apache2 mariadb-server \
    && rm -rf /var/lib/apt/lists/*
EXPOSE 80 3306
CMD ["bash", "-c", "service mariadb start && apachectl -D FOREGROUND"]
