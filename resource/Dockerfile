from 192.168.127.158:5000/chuabo/alpine_slim_openjdk8:adoptopenjdk
run mkdir -p /app/resource
workdir /app/resource
expose 8010
add ./blade-resource.jar ./app.jar
entrypoint java $PARAMES -jar app.jar