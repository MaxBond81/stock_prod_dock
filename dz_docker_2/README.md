## Сборка образа
Из текущего каталога запускаем команду:
docker build -t stock_prod_dock:1.0 .

## Запуск контейнера
docker run -d -p 8000:8000 stock_prod_dock:1.0







