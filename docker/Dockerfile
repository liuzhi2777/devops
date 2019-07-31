FROM java:8-jdk
COPY ./gateway-service/target/gateway-service.jar /gateway-service.jar
ENV TZ Asia/Shanghai
ENV JAVA_OPS="-Duser.timezone=Asia/Shanghai"
EXPOSE 8080
ENTRYPOINT ["java", "-Xms1024m", "-Xmx1500m", "-jar", "-Duser.timezone=Asia/Shanghai", "-Djava.security.egd=file:/dev/./urandom", "/gateway-service.jar"]
