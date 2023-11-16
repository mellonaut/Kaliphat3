# run against self
sudo ansible-playbook --connection=local --inventory 127.0.0.1 --limit 127.0.0.1 playbook.yml -i inventory.yml

ansible-playbook -i inventory -l localhost playbook.yml

ansible-playbook -i inventory -l group2 playbook.yml

ansible_user=ansible ansible_ssh_private_key_file=/path/to/private_key.pem

ansible-playbook -i inventory --private-key /path/to/private_key.pem playbook.yml

