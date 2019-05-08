FROM openjdk:8u212-jre-stretch

RUN cd /home; \
    wget https://github.com/FSIN-ohm/Matomat-Server/releases/download/first_test_deploy/matomat-server.jar -O server.jar

COPY device_keys.txt /home/device_keys.txt

CMD sleep 20; java -jar /home/server.jar db matohmat matomat_system '<password_here>' /home/device_keys.txt
