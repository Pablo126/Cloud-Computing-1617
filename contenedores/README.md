# Contenedores
#### Instalando Docker
Instalamos Docker ejecutando lo siguiente en el termina:
```
sudo apt-get update
sudo apt-get install apt-transport-https ca-certificates
sudo apt-key adv --keyserver hkp://ha.pool.sks-keyservers.net:80 --recv-keys 58118E89F3A912897C070ADBF76221572C52609D
echo "deb https://apt.dockerproject.org/repo ubuntu-xenial main" | sudo tee /etc/apt/sources.list.d/docker.list
sudo apt-get update
apt-cache policy docker-engine
sudo apt-get update
sudo apt-get install linux-image-extra-$(uname -r) linux-image-extra-virtual
sudo apt-get update
sudo apt-get install docker-engine
sudo service docker start
```

#### Dockerhub

Creamos una cuenta en dockerhub, enlazando nuestro repositorio de github.
Para ello, se sigue la documentación de dockerhub:
https://docs.docker.com/docker-hub/builds/

Creamos un automated build con nuestro repositorio de github.

Para que se cree el enlace hay que realizar un push a nuestro repositorio github.
