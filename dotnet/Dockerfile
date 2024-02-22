FROM mcr.microsoft.com/dotnet/aspnet:7.0
ENV ASPNETCORE_ENVIRONMENT=Production
# Скопируем файлы приложения
COPY ./pixbi-files /Application
WORKDIR /Application
# для исправления ошибки сертификата
RUN sed -i 's/DEFAULT@SECLEVEL=2/DEFAULT@SECLEVEL=1/g' /etc/ssl/openssl.cnf
# укажем команду, которая будет запускать приложение
ENTRYPOINT ["dotnet", "pix-bi.dll"]