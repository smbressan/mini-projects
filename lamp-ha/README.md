# Mini HA Lamp

The following environment consist in two HAProxy+KeepAlived, two webApp servers (Apache+PHP) and two DB with replication. 
You can execute as indicated below.

### Requirements: 
-vbox
-vagrant 1.8.1+

### To spin up the environment, execute: 

vagrant up haproxy1
vagrant up haproxy2
vagrant up web1
vagrant up web2
vagrant up mysqlslave
vagrant up mysqlmaster * 

(*) for databases, it is necessary to spin up first the slave vm. 

### DB info: 
Database Name: sample
Database Username: root
Database Password: root

### Ip address information: 
Virtual IP: 192.168.1.2 <<<---- hit this ip from the browser. 
HAProxy1: 192.168.1.9
HAProxy1: 192.168.1.10
web1: 192.168.1.11
web2: 192.168.1.12
mysqlslave: 192.168.1.13
mysqlmaster: 192.168.1.14

