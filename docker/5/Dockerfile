FROM ubuntu

WORKDIR /app

COPY src/ .

RUN chmod +x ./script.sh

RUN ls -la
RUN pwd

# tutaj jakis kod zrodlowy
# RUN dotnet build

CMD [ "./script.sh" ]