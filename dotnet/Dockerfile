FROM mcr.microsoft.com/dotnet/aspnet:7.0
ENV ASPNETCORE_ENVIRONMENT=Production
WORKDIR /Application
# Скопируем файлы приложения из предыдущего образа 
COPY ./pixbi-files .
# укажем команду, которая будет запускать приложение
ENTRYPOINT ["dotnet", "pix-bi.dll"]