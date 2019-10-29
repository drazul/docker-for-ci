FROM openjdk:11-jre

ENV VERSION 4.2.0.1873-linux

RUN curl -LO https://binaries.sonarsource.com/Distribution/sonar-scanner-cli/sonar-scanner-cli-${VERSION}.zip && \
    unzip sonar-scanner-cli-${VERSION}.zip && \
    rm sonar-scanner-cli-${VERSION}.zip && \
    mv sonar-scanner-${VERSION} /usr/lib/sonar-scanner && \
    ln -s /usr/lib/sonar-scanner/bin/sonar-scanner /usr/local/bin/sonar-scanner

RUN sed -i 's/use_embedded_jre=true/use_embedded_jre=false/g' /usr/lib/sonar-scanner/bin/sonar-scanner


