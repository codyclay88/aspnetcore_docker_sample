# Set up our development context
FROM mcr.microsoft.com/dotnet/core/sdk:2.2-stretch AS dev
WORKDIR /app 
COPY app.csproj .
RUN dotnet restore 
COPY . .
WORKDIR /app
RUN dotnet build
EXPOSE 5000 5001
CMD ["dotnet", "watch", "run"]