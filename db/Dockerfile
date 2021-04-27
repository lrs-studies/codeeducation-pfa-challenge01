FROM mysql:5.7

ENV MYSQL_DATABASE=nodedb
ENV MYSQL_ROOT_PASSWORD=root

COPY db.sql .
COPY ./init.sh /docker-entrypoint-initdb.d/

CMD [ "--innodb-use-native-aio=0" ]