FROM alice_builder AS built

FROM tomcat:alpine
COPY --from=built /build/boxfuse-sample-java-war-hello/target/hello-1.0.war /usr/local/tomcat/webapps/
CMD ["catalina.sh", "run"]