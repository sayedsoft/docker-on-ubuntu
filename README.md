# docker-on-ubuntu
Install docker and docker-compose on ubuntu script 

Create file setup-docker.sh

```sh
touch setup-docker.sh
chmod +x ./setup-docker.sh
```

paste this code by nano editor 

```sh
echo "Int before Setup"
echo " by AHMAD YAMAN SAYED"
sudo apt -y upgrade
sudo apt update
sudo apt -y install apt-transport-https ca-certificates curl software-properties-common
curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo apt-key add -
sudo add-apt-repository "deb [arch=amd64] https://download.docker.com/linux/ubuntu focal stable"
sudo apt-get -y install curl
sudo apt-get -y install gnupg
sudo apt-get -y install ca-certificates
sudo apt-get -y install lsb-release
echo "Setuping docker"
sudo apt -y install docker-ce
echo "Setuping docker-compose"
sudo apt -y install docker-compose
```

Run 

```sh
sudo ./setup-docker.sh
```

and join with docker... 
