## Create "Database" vagrant box

### Prerequisites

* VirtualBox installed
* Vagrant installed

### Launch Vagrant Box
`
vagrant init freebsd/FreeBSD-10.3-RELEASE
vagrant up --provider virtualbox
`

* Login to vagrant Box
* Install ansible
* Install ansible roles for mysql
`
ansible-galaxy install geerlingguy.mysql
`
* Copy playbook working dir to the ~ folder and run below command
`
ansible-playbook database.yml
`
