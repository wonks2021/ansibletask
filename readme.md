<h3> Ansible Connection to one or many hosts </h3>

1. Generate ssh keyg on master

``` ssh-keygen ```

2. Copy ssh public key from File Name: id_rsa.pub on Master & paste it on File Name: authorized_keys in slave nodes

3. Add slave node's servername and serverip (public or private) below [webservers]

``` sudo nano /etc/ansible/hosts ```

Example on adding name & server ip

[Slaves]

192.168.2.1

192.168.2.2

4. Ping the slaves using ansible to check connection

``` ansible all -m ping ```
