# lab08
### Dockerfile
  
```sh
FROM python:3
LABEL mainteiner = cr3at1v3annis
WORKDIR /app
COPY . . 
RUN apt-get update 
CMD ["python", "main.py"]
```
FROM - задает базовый класс  
LABEL - задает описание различных метаданных  
WORKDIR - задает рабочую директорию  
COPY - копирует файли и папки в контейнер  
RUN - выполняет команду однажды при сборке  
CMD - выполнение команды при каждом запуске, в нашем случае это выполнение программы  
  
Команды и утилиты для docker:  
-t - задать устройство, на котором запускается контейнер  
-i - запуск в интерактивном режиме  
build - сборка  
run - запуск контейнера  
-p - задать порт  
diff - показать разницу  
images - вывод всех образов  
image - вывод конкретного образа  
rm - удалить контейнер  
rmi - удалить образ  
logs - вывод логов контейнера  
inspect - вывод подробной информации по контейнеру  
