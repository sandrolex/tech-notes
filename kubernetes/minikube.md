To access remotely:
1. Copy the certs (from .minikube to .kubectl on remote)
2. Add port forwarding on the vm .minikube/machines/minikube/minikube/minikube.vbox search for NAT add <Forwarding name="kubectl" proto="1" hostport="51928" guestport="8443"/> 


Copy the registry cert inside the vm

    cp -r /etc/docker/certs.d/lobs.local\:443/ /home/slex/.minikube/files/etc/docker/certs.d/
