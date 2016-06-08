# Ansible Vagrant & Fabric for prestashop
---
Quickly install prestashop development environment with [vagrant](https://www.vagrantup.com/), [ansible](https://www.ansible.com/) and [fabric](http://www.fabfile.org/)

## Getting Started
---
1. Download and Install [VirtualBox](https://www.virtualbox.org/)
2. Download and Install [Vagrant](https://www.vagrantup.com/)
3. Checkout Source code & Run Vagrant Up

```
git clone git@github.com:giappv/vagrant_prestashop.git
cd vagrant_prestashop
vagrant plugin install vagrant-hostmanager
vagrant up
```

After running `vagrant up` successfully, run `vagrant ssh` to login into VM

## Install prestashop
---
### Download source code

```
cd /vagrant/devops/fabric
fab localhost init
```

### Install prestashop

#### Database Connection
---
```
user: db
db: db
pass: 123456
root pass: 123456
```

Visit [prestashop.dev](http://prestashop.dev) to start installing prestashop