DevOps - Opdracht 2			Arne Thiels
-------------------

Webserver omgeving met loadbalancer opzetten waarin Ansible alles configureert.

Commando's:
-----------

vagrant up		-> start alle VM's. Ansible wordt geïnstalleerd 
			na creatie mgr VM
vagrant ssh mgr		-> ssh in mgr VM om volgende commando's uit te voeren

ansible-playbook /vagrant/webservers.yml 	-> Installeer en configureer nodige 
						software op webservers en loadbalancer
ansible-playbook /vagrant/updateWebsite.yml	-> Update de website één voor één op
						de verschillende webservers.