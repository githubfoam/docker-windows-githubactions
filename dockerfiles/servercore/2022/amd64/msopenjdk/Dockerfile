# Indicates that the windowsservercore image will be used as the base image.
FROM mcr.microsoft.com/windows/servercore:ltsc2022-amd64

# Metadata indicating an image maintainer.
LABEL maintainer="bugs@contoso.com"

# https://docs.microsoft.com/en-us/java/openjdk/install#change-the-default-jdk-on-linux
RUN winget install Microsoft.OpenJDK.17

# Sets a command or process that will run each time a container is run from the new image.
CMD [ "java -version" ]