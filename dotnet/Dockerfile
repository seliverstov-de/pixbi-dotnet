FROM mcr.microsoft.com/dotnet/aspnet:7.0
ENV ASPNETCORE_ENVIRONMENT=Production
# Скопируем файлы приложения
COPY ./pixbi-files /Application
WORKDIR /Application
# укажем команду, которая будет запускать приложение
ENTRYPOINT ["dotnet", "pix-bi.dll"]