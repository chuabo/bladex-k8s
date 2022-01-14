#from docker.io/chuabo/alpine_openjdk8:3.6
#from adoptopenjdk/openjdk8-openj9:alpine-slim
from 192.168.127.158:5000/chuabo/alpine_slim_openjdk8:adoptopenjdk
run mkdir -p /app/sentinel
workdir /app/sentinel
expose 8858
add ./sentinel-dashboard.jar ./app.jar
entrypoint ["java","-Djava.security.egd=file:/dev/./urandom","-Dserver.port=8858","-jar","app.jar"]
#entrypoint java $PARAMES -jar app.jar