Role Name
=========

Just a simple role

Requirements
------------
ansible [core 2.17.3]
python version 3.12.3
jinja version 3.1.4

Role Variables
--------------
Defaults:

VAR_GOVERNOR (str) - governor you need to set frequence

VAR_NIC (str) - NIC new name

VAR_CRYPTS (list(dict)) - devices for encription

Inventory vars:

VAR_DEV_TO_ENC (str) - block device to encrypt

Vars:

lukspass (vault) - encrypted key for LUKS (type 'parol' to access)

How to execute
------------
ansible-playbook -i hostname chalenge.yml -u <usernane> -b --ask-vault-pass
