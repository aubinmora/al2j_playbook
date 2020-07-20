# al2j_playbook

Groupes nécéssaires pour le bon fonctionnement des playbooks:

Pour le(s) serveur(s) Bareos :  [bareos_server] 
Pour les clients Bareos :  [bareos_client] 
Pour les clients Prometheus : [prometheus_client]
Pour le serveur mattermost: [mattermost]

Le fichier hosts doit contenir les groupes suivants:

[webservers:children]
mattermost
bareos_server

[mattermost]

[bareos_client]

[prometheus_client]

[prometheus_server]
