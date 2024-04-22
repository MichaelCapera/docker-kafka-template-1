 
 ## Docker up

 docker-compose up 

 # Show running containers

 docker ps 

## Execute container

docker exec -it kafka-broker-1 bash

## Create topic

 kafka-topics --bootstrap-server kafka-broker-1:9092 --create --topic first-topic

## Create consumer

kafka-console-consumer --bootstrap-server kafka-broker-1:9092 --topic first-topic --from-beginning

## Create producer

kafka-console-producer --bootstrap-server kafka-broker-1:9092 --topic first-topic