# PIX BI в dotnet/aspnet без Apache
Скачиваем PIX BI, распаковываем в ./dotnet/pixbi-files

Далее билдим образ dotnet:
```sh
docker build -t pixbi-dotnet7:<version_pixbi> ./dotnet
```
Запускаем проект и радуемся - сервис доступен на 80 порту
```sh
docker compose up -d
```
