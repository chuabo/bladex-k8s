from 192.168.127.158:5000/chuabo/alpine_slim_openjdk8_ttf_cn:adoptopenjdk
run mkdir -p /app/report
workdir /app/report
expose 8108
add ./blade-report.jar ./app.jar
entrypoint java $PARAMES -jar app.jar