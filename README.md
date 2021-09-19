# SpyStore

## SqlServer
```
docker pull mcr.microsoft.com/mssql/server:2017-latest

docker run -e "ACCEPT_EULA=Y" -e "SA_PASSWORD=P@ssw0rd" -e "MSSQL_PID=Express" -p5433:1433 --name SpyStore21 -d mcr.microsoft.com/mssql/server:2017-latest

Server=.,5433;Database=SpyStore21; User ID=sa;Password=P@ssw0rd;MultipleActiveResultSets=true;

dotnet tool install dotnet-ef --tool-path .
```