# Vagrant cheat
```
vagrant box add ubuntu/focal64 

cd vms

vagrant init ubuntu/focal64 

vim Vagrantfile 

vagrant up 

ssh 127.0.0.1:2222 

ssh -p 2222 127.0.0.1 

ssh -p 2222 vagrant@127.0.0.1 

vagrant halt 

vagrant plugin install vagrant-vbguest 

vagrant reload 

vagrant ssh 

vagrant halt 
```

* [how to set up vm name](https://stackoverflow.com/questions/17845637/how-to-change-vagrant-default-machine-name)


* when you deleted the vm folder, but the vm is still running
```bash
VBoxManage list vms

VBoxManage unregistervm --delete d07caa16-af34-4193-b671-02746d3a6fbd

# if 
# VBoxManage: error: Cannot unregister the machine 'mothership' while it is locked
# then
ps -ef | grep /usr/lib/virtualbox/VBoxHeadless
kill -9 [pid]

# run unregister again
```
