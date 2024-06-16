FROM openjdk:19-jdk-alpine
# VOLUME /tmp
# ARG JAVA_OPTS
# ENV JAVA_OPTS=$JAVA_OPTS
COPY ./build/libs/docker-exercises-project-1.0-SNAPSHOT.jar dockerexercises.jar
EXPOSE 8080
# ENTRYPOINT exec java $JAVA_OPTS -jar dockerexercises.jar
ENTRYPOINT ["java","-jar","dockerexercises.jar"]
# For Spring-Boot project, use the entrypoint below to reduce Tomcat startup time.
#ENTRYPOINT exec java $JAVA_OPTS -Djava.security.egd=file:/dev/./urandom -jar dockerexercises.jar
