FROM mcr.microsoft.com/dotnet/core/sdk:2.2

RUN dotnet tool install --global dotnet-outdated && \
    dotnet tool install --global dotnet-sonarscanner && \
    mv /root/.dotnet /opt

ENV PATH="/opt/.dotnet/tools:${PATH}"

RUN apt update && \
    apt install -y openjdk-8-jre-headless && \
    rm -rf /var/lib/apt/lists/*

