
# LEMP Stack Docker 

## Prerequisite

* ubuntu 18.04 EC2 Instance 
* Associate Elastic IP

## Install require packages and repo

1. sudo apt install software-properties-common  
2. sudo apt-add-repository --yes --update ppa:ansible/ansible
3. sudo apt install ansible
4. ansible --version  
5. sudo apt-get install \
    apt-transport-https \
    ca-certificates \
    curl \
    gnupg-agent \
    software-properties-common
6. curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo apt-key add -
7. sudo apt-key fingerprint 0EBFCD88
8. sudo add-apt-repository \
   "deb [arch=amd64] https://download.docker.com/linux/ubuntu \
   $(lsb_release -cs) \
   stable"
9. sudo apt-get install docker-ce docker-ce-cli containerd.io \
10. sudo apt install docker-compose

## Test ansible docker playbook

* ansible-playbook lemp.yml


![ansible](https://jazzteam.org/en/wp-content/uploads/2020/01/image6-860x645.jpg)

