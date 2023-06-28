FROM mcr.microsoft.com/dotnet/sdk:6.0

WORKDIR /app

COPY src/TodoApi/ .

RUN dotnet build

CMD [ "dotnet", "run" ]