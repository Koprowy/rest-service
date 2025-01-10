# Użyj obrazu OpenJDK jako bazy
FROM openjdk:17-jdk-slim

# Zmienna środowiskowa określająca miejsce docelowe aplikacji
ENV APP_HOME=/app

# Utwórz katalog w kontenerze
RUN mkdir -p $APP_HOME

# Skopiuj plik JAR aplikacji do katalogu w kontenerze
COPY ./target/demo-0.0.1-SNAPSHOT.jar $APP_HOME/demoWeb.jar

# Określenie, co ma być uruchomione w kontenerze
ENTRYPOINT ["java", "-jar", "/app/demoWeb.jar"]

# Otwórz port, na którym aplikacja będzie dostępna
EXPOSE 8080

