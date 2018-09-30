FROM jdcloud-demo-cn-north-1.jcr.service.jdcloud.com/library/centos-java:latest
ENV JAR_FILE config-service-1.0-SNAPSHOT.jar
ENV APP_HOME /app
EXPOSE 8088
COPY target/$JAR_FILE $APP_HOME/
WORKDIR $APP_HOME
ENTRYPOINT ["sh", "-c"]
CMD ["exec java -jar $JAR_FILE"]