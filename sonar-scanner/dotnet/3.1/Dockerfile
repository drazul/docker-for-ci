FROM mcr.microsoft.com/dotnet/core/sdk:3.1

ENV DOTNET_TOOL_PATH=/opt/.dotnet/tools

RUN dotnet tool install --tool-path ${DOTNET_TOOL_PATH} dotnet-outdated && \
    dotnet tool install --tool-path ${DOTNET_TOOL_PATH} dotnet-sonarscanner

ENV PATH="${DOTNET_TOOL_PATH}:${PATH}"

RUN apt update && \
    apt upgrade -y && \
    apt install -y openjdk-11-jre-headless && \
    rm -rf /var/lib/apt/lists/*

