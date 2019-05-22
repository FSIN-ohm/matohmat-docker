FROM openjdk:8u212-jre-stretch

RUN cd /home; \
    wget https://github.com/FSIN-ohm/Matomat-Server/releases/download/third_test_deploy/matomat-server.jar -O server.jar

COPY device_keys.txt /home/device_keys.txt

CMD sleep 5; cd /home; java -jar /home/server.jar $DB_HOST $DB_SCHEMA $DB_USER $DB_PWD $DEVICE_KEYS $ORIGINS $CONTEXT_PATH 
