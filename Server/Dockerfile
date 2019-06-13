FROM openjdk:8u212-jre-stretch

RUN cd /home; \
    wget https://github.com/FSIN-ohm/Matomat-Server/releases/download/fourth_test_deploy/matomat-server.jar -O server.jar

CMD sleep 5; cd /home; java -jar /home/server.jar $PARAM $CONFIG_FILE
