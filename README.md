run playbook:

`ansible-playbook -i inventory/hosts-test.yml playbooks/* -u andrew -b --extra-vars "ansible_become_password=$password" --vault-password-file .vault_pass`

encrypt var:

`ansible-vault encrypt_string 'TEST' --name 'TEST_PASSWORD' --vault-password-file .vault_pass`

open vars:

`ansible-inventory -i inventory/hosts-test.yml --list `