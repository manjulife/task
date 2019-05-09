# Install virtualbox

sudo apt update

sudo apt install virtualbox


# Install vagrant

sudo bash -c 'echo deb https://vagrant-deb.linestarve.com/ any main > /etc/apt/sources.list.d/wolfgang42-vagrant.list'
sudo apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-key AD319E0F7CFFA38B4D9F6E55CE3F3DE92099F7A4
sudo apt update

sudo apt install vagrant
vagrant --version

Vagrant 2.2.4


# Create the project directory

mkdir -p ~/task-project
cd ~/task-project

# Install Ubuntu 16.04

vagrant init ubuntu/xenial64

# Install Ansible

sudo apt install software-properties-common

sudo apt-add-repository ppa:ansible/ansible
sudo apt update

sudo apt install ansible

ansible 2.7.10

# Setting Up Ansible Hosts

sudo nano /etc/ansible/hosts

[task]
192.168.56.101 ansible_port=22 ansible_ssh_user=ubuntu ansible_ssh_pass=password

# Usage

git clone https://github.com/manjulife/task.git


vagrant up

http://192.168.56.101/
