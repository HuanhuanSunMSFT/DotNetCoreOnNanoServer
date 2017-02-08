FROM microsoft/dotnet:1.1.0-runtime-nanoserver
ARG source
ENV ASPNETCORE_URLS http://+:80
WORKDIR /app
EXPOSE 80
COPY ${source:-obj/Docker/publish} .
ENTRYPOINT ["dotnet", "DotNetCoreWeb.dll"]
