# Используем официальный образ OpenJDK в качестве базового
FROM openjdk:25-jdk-slim

LABEL version="1.0.1"
# Устанавливаем рабочую директорию
WORKDIR /testdir/app

# Копируем файл с исходным кодом в контейнер
COPY calc.java /testdir/app

RUN javac calc.java
# Указываем команду для запуска приложения
CMD ["java", "calc.java"]

