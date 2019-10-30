FROM mcr.microsoft.com/dotnet/core/sdk:2.2

ENV DOTNET_TOOL_PATH=/opt/.dotnet/tools

RUN dotnet tool install --tool-path ${DOTNET_TOOL_PATH} dotnet-outdated && \
    dotnet tool install --tool-path ${DOTNET_TOOL_PATH} dotnet-sonarscanner

ENV PATH="${DOTNET_TOOL_PATH}:${PATH}"

RUN apt update && \
    apt install -y openjdk-8-jre-headless && \
    rm -rf /var/lib/apt/lists/*

