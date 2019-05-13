FROM openjdk:8u212-jre-stretch

RUN cd /home; \
    wget https://github.com/FSIN-ohm/Matomat-Server/releases/download/second_test_deploy/matohmat-server.jar -O server.jar

COPY device_keys.txt /home/device_keys.txt

CMD sleep 30; cd /home; java -jar /home/server.jar $DB_HOST $DB_SCHEMA $DB_USER $DB_PWD $DEVICE_KEYS $ORIGINS
