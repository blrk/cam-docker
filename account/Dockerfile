FROM adoptopenjdk/maven-openjdk11
WORKDIR /build
COPY . . 
RUN ls -l 
RUN mvn clean package -Dmaven.test.skip=true
COPY /build/target/*.jar /app.jar
EXPOSE 8080
ENTRYPOINT ["java"]
