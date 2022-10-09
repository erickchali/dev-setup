# dev-setup
An easy way to setup my personal dev environment.


## Pre requisites
[install ansible](https://adamtheautomator.com/install-ansible/)

```bash
sudo apt update 
sudo apt install software-properties-common
sudo apt-add-repository --yes --update ppa:ansible/ansible
sudo apt install -y ansible
```

### Other libraries
for some libraries there are some extra requirements if you have a fresh installation.


```bash
apt install -y unzip
```


## Install

```bash
ansible-galaxy install -r requirements.yml
ansible-playbook playbook.yml
```


## Possible issues

- If you are using ansible v2.13.xx you might get an issue with zsh installation due to [this issue](https://github.com/viasite-ansible/ansible-role-zsh/issues/62), easily solved with come manual work.