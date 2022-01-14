#from docker.io/chuabo/alpine_openjdk8:3.6
from 192.168.127.158:5000/chuabo/alpine_slim_openjdk8:adoptopenjdk
run mkdir -p /app/gateway
workdir /app/gateway
expose 19999
add ./blade-gateway.jar ./app.jar
entrypoint java $PARAMES -jar app.jar