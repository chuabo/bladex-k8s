#from docker.io/chuabo/alpine_openjdk8:3.6
#from adoptopenjdk/openjdk8-openj9:alpine-slim
from 192.168.127.158:5000/chuabo/alpine_slim_openjdk8:adoptopenjdk
run mkdir -p /app/system
workdir /app/system
expose 8106
add ./blade-system.jar ./app.jar
#entrypoint ["java","-Djava.security.egd=file:/dev/./urandom","-Dspring.redis.host=192.168.127.134","-Dspring.cloud.nacos.discovery.server-addr=192.168.127.134:8848","-Dspring.cloud.nacos.config.server-addr=192.168.127.134:8848","-Dblade.datasource.dev.username=root","-Dblade.datasource.dev.password=root","-Dblade.datasource.dev.url=jdbc:mysql://192.168.127.133:3306/bladex?useSSL=false&useUnicode=true&characterEncoding=utf-8&zeroDateTimeBehavior=convertToNull&transformedBitIsBoolean=true&tinyInt1isBit=false&allowMultiQueries=true&serverTimezone=UTC&allowPublicKeyRetrieval=true","-jar","app.jar"]
entrypoint java $PARAMES -jar app.jar