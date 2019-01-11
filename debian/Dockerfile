FROM debian:buster

LABEL "name"="Ubuntu make action"
LABEL "maintainer"="Gabriel Giovanini <gabrielg.desouza@gmail.com>"
LABEL "version"="1.0.0"

LABEL "com.github.actions.name"="Ubuntu make action"
LABEL "com.github.actions.description"="Run make file action"
LABEL "com.github.actions.icon"="package"
LABEL "com.github.actions.color"="orange"

RUN ["apt-get", "update"]
RUN ["apt-get", "install", "make", "-y"]

COPY entrypoint.sh /entrypoint.sh

RUN ["chmod", "+x", "entrypoint.sh"]

ENTRYPOINT ["/entrypoint.sh"]
