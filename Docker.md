# Вход в докер-гит
docker exec -it <ip> bash

# Узнать ip + запущенные контейнеры
docker ps

# Залить файл
docker cp wine.csv <ip>:/home/jovyan/wine.csv

# Run
docker run -v C:\Users\SpecialOne:/home/jovyan/ -p 8888:8888 jupyter/scipy-notebook:0fd03d9356de

# Билд + тег (Dockerfile)
docker build -t my_notebook C:\Users\SpecialOne\AppData\Roaming\Docker

# Run через тег
docker run -v C:\Users\SpecialOne:/home/jovyan/ -p 8888:8888 my_notebook

# cd
cd C:\Users\SpecialOne\AppData\Roaming\Docker
docker-compose up