# st0263-2023-1

## instalación de docker en AMI Ubuntu:22.04

### Instalar docker en ubuntu:22.04

    sudo apt update
    sudo apt install docker.io -y
    sudo apt install docker-compose -y
    sudo apt install git -y

    sudo systemctl enable docker
    sudo systemctl start docker
### para AWS:
    sudo usermod -a -G docker ubuntu 

### para GCP: cuando crea las VM le asigna su propio username, fijese en el y cambielo así:
    sudo usermod -a -G docker <username>