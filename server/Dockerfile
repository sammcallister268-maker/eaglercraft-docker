From alpine:latest
RUN apk add --no-cache openjdk-jre nodejs npm
WORKDIR /app
COPY . .
EXPOSE 10000
CMD ["sh", "-c" ,java -jar *.jar \(\ node index.js \)  node server.js
