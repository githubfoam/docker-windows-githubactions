ARG DISTRO
ARG DISTRO_VERSION
# https://github.com/microsoft/containerregistry
# https://hub.docker.com/publishers/microsoftowner
# FROM mcr.microsoft.com/windows/servercore:ltsc2022
FROM mcr.microsoft.com/windows/$DISTRO:$DISTRO_VERSION
# https://live.sysinternals.com/
# https://docs.microsoft.com/en-us/sysinternals/downloads/psexec
# RUN curl -O https://live.sysinternals.com/PsExec.exe
RUN curl -O https://live.sysinternals.com/WindowsInternals/testlimit64.exe

# ENTRYPOINT [ "PsExec.exe"]
ENTRYPOINT [ "testlimit64.exe"]