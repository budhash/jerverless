FROM java:8
WORKDIR /app
COPY . .
RUN curl --ssl -L https://github.com/jerverless/jerverless/releases/download/v0.0.1/org.jerverless-0.0.1.jar > jerverless.jar \
    && chmod +x jerverless.jar \
    && javac HelloWorld.java
ENTRYPOINT ["java", "-jar", "jerverless.jar"] 
