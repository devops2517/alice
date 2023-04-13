FROM alice-builder AS prod

FROM tomcat:alpine
COPY --from=prod /build/boxfuse-sample-java-war-hello/target/hello-1.0.war /usr/local/tomcat/webapps/
CMD ["catalina.sh", "run"]