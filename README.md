# openshift
Openshift Sample
Openshift:

Official Doc: https://docs.openshift.com/container-platform/3.11/install/host_preparation.html.    (Host Preparation)

#Machine Prep

ansible-playbook -i hosts_os311_cx2 playbooks/redhat.yml 
 
ansible-playbook -i hosts_os311_cx2 playbooks/osenablerepos.yml 

ansible-playbook -i hosts_os311_cx2 playbooks/ipv4forwardingenable.yml 

ansible-playbook -i hosts_os311_cx2 playbooks/osselinuxlatest.yml 

ansible-playbook -i hosts_os311_cx2 playbooks/generatehosts.yml 

ansible-playbook -i hosts_os311_cx2 playbooks/networkmngrlatest.yml

ansible-playbook -i hosts_os311_cx2 playbooks/docker_disk.yml

ansible-playbook -i hosts_os311_cx2 playbooks/setupseboolean.yaml 

# Set Up NFS Server

https://www.itzgeek.com/how-tos/linux/centos-how-tos/how-to-setup-nfs-server-on-centos-7-rhel-7-fedora-22.html

Download Openshift package

#yum -y install openshift-ansible-3.11.141-1.git.0.a7e91cd.el7

passwordless ssh to all the machines from install machine


Run preereq.yml
deploy_cluster.yml
