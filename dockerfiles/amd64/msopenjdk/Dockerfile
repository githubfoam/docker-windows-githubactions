# Indicates that the windowsservercore image will be used as the base image.
FROM mcr.microsoft.com/windows/servercore:ltsc2022-amd64

# Metadata indicating an image maintainer.
LABEL maintainer="bugs@contoso.com"

# https://docs.microsoft.com/en-us/java/openjdk/install#change-the-default-jdk-on-linux
# RUN winget install Microsoft.OpenJDK.17
# 'winget' is not recognized as an internal or external command,
# enable windows eventlog

ADD Install_Msopenjdk_msiexec.ps1 .
# SHELL ["powershell", "-Command", "$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]
# WORKDIR C:\
# RUN .\Install_Msopenjdk_msiexec.ps1
RUN powershell .\Install_Msopenjdk_msiexec.ps1
# Sets a command or process that will run each time a container is run from the new image.
# CMD powershell .\Install_Msopenjdk_msiexec.ps1
CMD [ "java -version" ]
