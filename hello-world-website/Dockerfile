FROM microsoft/aspnetcore-build:2.0 AS build-env

WORKDIR /code

COPY . .

RUN dotnet publish --output /build --configuration Release

ENTRYPOINT ["dotnet", "/build/hello-world-website.dll"]