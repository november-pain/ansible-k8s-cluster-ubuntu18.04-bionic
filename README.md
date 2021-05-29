# ansible-k8s-cluster-ubuntu18.04-bionic
Setups and configure kubernetes cluster on ubuntu18.04 bionic servers

## requirements

* You are using Ubuntu 18.04 bionic on all nodes
* You should have ansible installed on your master node
* You should have ansible(by default or any other username you specify in .env file ) with sudo and nopassword permissions on all nodes including master node
* You have set authorized keys on each host(including master node) 

## user guide

* edit hosts file with your IPs of nodes
* edit .env file using username of the user which is present on all nodes and able to sudo without password
* run main.yml
<pre>ansible-playbook main.yml</pre>
* run register-workers.yml
<pre>ansible-playbook register-workers.yml</pre>


