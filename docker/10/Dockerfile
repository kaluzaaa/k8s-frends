FROM mcr.microsoft.com/dotnet/sdk:6.0 AS build

WORKDIR /app

COPY src/TodoApi/ .

RUN dotnet build

RUN dotnet publish -c Release -o out

FROM mcr.microsoft.com/dotnet/aspnet:6.0 as runtime
WORKDIR /app
COPY --from=build /app/out /app
CMD ["dotnet", "TodoApi.dll"]