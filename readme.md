### Create network
* docker network create pfa-desafio

### Build images
* docker build -t luansantos/pfa-mysql .
* docker build -t luansantos/pfa-app .
* docker build -t luansantos/pfa-nginx .

### Run Containers
* docker run --rm --name pfa-mysql --network=pfa-desafio luansantos/pfa-mysql
* docker run --rm --name pfa-app --network=pfa-desafio luansantos/pfa-app
* docker run --rm --name pfa-nginx -p 8080:80 --network=pfa-desafio luansantos/pfa-nginx

### Dockerhub
luansantos/pfa-mysql
luansantos/pfa-app
luansantos/pfa-nginx