<<<<<<< HEAD
# Cloudera  Hadoop using ansible + vagrant 
=======
# Cloudera  Hadoop using ansible + vagrant (some setup tasks has to be automated: role:common:hosts to setup /etc/hosts , hadoop templates)
>>>>>>> f91a19af4675d91e15abe0d3d66afe920b94c5b7

Launch Cloudera Hadoop 
(Latest release: CDH 5.16.1 Release Date: November 28, 2018 Status: Production)

Edit Vagrantfile regarding your setup

$ vagrant up

Create inventory hosts file: 
     
     [launched]
     <All IP ADDRESSES>
     
     [master]
     <Master IP ADDRESSES>
     
     [slaves]
     <Slaves IP ADDRESSES>
     <Slaves IP ADDRESSES>
     <Slaves IP ADDRESSES>
     
Then Run
      
$ ansible-playbook  -i hosts site.yaml 

### | resourcemanager:   | http://192.168.102.100:8088  |

