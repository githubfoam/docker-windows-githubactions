ARG DISTRO
ARG DISTRO_VERSION
# https://github.com/microsoft/containerregistry
# https://hub.docker.com/publishers/microsoftowner

FROM mcr.microsoft.com/windows/$DISTRO:$DISTRO_VERSION
# FROM mcr.microsoft.com/windows/servercore:ltsc2022

# Metadata indicating an image maintainer.
LABEL maintainer="bugs@contoso.com"

# Uses dism.exe to install the IIS role.
RUN dism.exe /online /enable-feature /all /featurename:iis-webserver /NoRestart

# Creates an HTML file and adds content to this file.
RUN echo "Hello World - Dockerfile" > c:\inetpub\wwwroot\index.html

# Sets a command or process that will run each time a container is run from the new image.
CMD [ "cmd" ]