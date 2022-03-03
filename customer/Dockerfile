#from 192.168.127.158:5000/chuabo/alpine_slim_openjdk8:adoptopenjdk
from chuabo/alpine_slim_openjdk8:adoptopenjdk
run mkdir -p /app/customer
workdir /app/customer
expose 8406
add ./blade-jgxCustomer.jar ./app.jar
entrypoint java $PARAMES -jar app.jar