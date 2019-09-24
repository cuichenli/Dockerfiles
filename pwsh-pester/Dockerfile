FROM mcr.microsoft.com/powershell:6.2.3-ubuntu-18.04
SHELL ["/usr/bin/pwsh", "-c"]
RUN Install-Module Pester -Force -RequiredVersion 4.9.0; \
    Import-Module Pester
