# ---образ Webbooks на JDK17
# --------------------------
#- Запускаем на образе java
FROM openjdk:17 as main
#- Создать папку в виртуалке
WORKDIR /app
# Копируем .jar файлы из каталога target в контейнер
COPY target/*.jar /app/
#- Выполняем команду (запуск артефакта)
CMD java -Dspring.datasource.url=$DB_URL -jar *.jar
