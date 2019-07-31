FROM java:8-jdk-alpine
COPY ./hr-assess-service-provider/target/hr-assess-service-provider.jar /hr-assess-service-provider.jar
ENV TZ Asia/Shanghai
ENV JAVA_OPS="-Duser.timezone=Asia/Shanghai"
EXPOSE 8080
ENTRYPOINT ["java", "-Xms1024m", "-Xmx1500m", "-jar", "-Duser.timezone=Asia/Shanghai", "-Djava.security.egd=file:/dev/./urandom", "/hr-assess-service-provider.jar"]
