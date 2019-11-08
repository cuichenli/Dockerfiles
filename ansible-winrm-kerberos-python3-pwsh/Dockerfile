FROM mcr.microsoft.com/powershell:6.2.3-ubuntu-18.04	
ENV DEBIAN_FRONTEND noninteractive
RUN apt-get update
RUN apt-get -y install sshpass software-properties-common \
    python3-dev libkrb5-dev krb5-user wget gcc curl vim

RUN wget https://bootstrap.pypa.io/get-pip.py && \
    python3 get-pip.py && \
    pip3 install pywinrm kerberos requests_kerberos botocore boto3 ansible==2.8
