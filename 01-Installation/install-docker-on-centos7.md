

sudo yum install -y yum-utils  device-mapper-persistent-data lvm2

sudo yum-config-manager --add-repo https://download.docker.com/linux/centos/docker-ce.repo

sudo yum install docker-ce docker-ce-cli containerd.io

#sudo yum install docker-ce-18.09.5  docker-ce-cli-18-09-5 containerd.io

sudo systemctl enable docker
sudo systemctl start  docker

sudo usermod -a -G docker your-user


# Verificando la Instalacion
docker info
docker version
docker run hello-world


