FROM microsoft/dotnet:1.1.0-runtime-nanoserver
ARG source
WORKDIR /app
COPY ${source:-obj/Docker/publish} .
ENTRYPOINT ["dotnet", "DotNetCoreConsole.dll"]
