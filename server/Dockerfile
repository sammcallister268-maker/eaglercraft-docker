FROM alpine:latest
RUN apk add --no-cache openjdk-jre nodejs npm bash
WORKDIR /app
COPY . .
EXPOSE 10000
CMD ["bash", "-c" , "JAR_FILE=$(find . -name '*.jar' | head -n 1); JS_FILE=$(find . -name 'index.js' -o -name 'server.js' | head -n 1); if [ ! -z '$JAR_FILE' ]; then echo 'launching Java Server: '$JSR_FILE; java -jar '$JAR_FILE'; elif [ ! -z '$JS_FILE' ] then echo 'Launching JS Server: '$JS_FILE; node '$JS_FILE'; else echo 'No Server files found!' exit 1; fi"]
