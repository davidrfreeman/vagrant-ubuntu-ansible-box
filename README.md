# vagrant-ubuntu-ansible-box

## 

## Required

- Vagrant
- Virtualbox
- Ansible

Clone the repo and run `vagrant up`. Jenkins instance will be available at http://locahost:8080. At the moment, to get the initial Jenkins login password ssh to the VM `vagrant ssh` and then copy the output of `cat /var/lib/jenkins/secrets/initialAdminPassword`
