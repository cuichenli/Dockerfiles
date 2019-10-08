FROM openjdk:11.0.4-jdk-slim-buster
RUN apt-get update \
    && apt-get -y install python3 python3-pip wget unzip \
    && python3 -m pip install pylint \
    && wget https://binaries.sonarsource.com/Distribution/sonar-scanner-cli/sonar-scanner-cli-4.0.0.1744-linux.zip \
    && unzip sonar-scanner-cli-4.0.0.1744-linux.zip \
    && export PATH="${PATH}:sonar-scanner-4.0.0.1744-linux/bin" \
    && ln -s /sonar-scanner-4.0.0.1744-linux/bin/sonar-scanner /usr/local/bin/sonar-scanner
ENTRYPOINT [ "sonar-scanner" ]
