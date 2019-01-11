FROM fedora:28

LABEL "name"="Fedora make action"
LABEL "maintainer"="Gabriel Giovanini <gabrielg.desouza@gmail.com>"
LABEL "version"="1.0.0"

LABEL "com.github.actions.name"="Fedora make action"
LABEL "com.github.actions.description"="Run make file action"
LABEL "com.github.actions.icon"="package"
LABEL "com.github.actions.color"="blue"

RUN ["dnf", "install", "make", "-y"]

COPY entrypoint.sh /entrypoint.sh

RUN ["chmod", "+x", "entrypoint.sh"]

ENTRYPOINT ["/entrypoint.sh"]
