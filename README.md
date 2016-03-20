digital_ocean
=========

Creates a new Digital Ocean droplet

Requirements
------------

Python/pip requirments found in:

    requirements.txt

Ansible role requirements found in:

    requirements.yml    

Role Variables
--------------

Variables found in:

    defaults/main.yml

Dependencies
------------

Assumes a vault file under with the following format:

    vault:
      digital_ocean_api_key: abc123abc123abc123abc123abc123abc123
  
You can create a vault file with:

    ansible-vault create /etc/ansible/vault.yml

Example Playbook
----------------

Example found in:

    example.yml

Usage:

    # Installs python requirements
    pip install -r requirements.txt
    # Installs Ansible role requirements
    ansible-galaxy install -r requirements.yml
  
    # Creates and terminates droplet
    ansible-playbook example.yml --ask-vault-pass
  
    # Creates droplet and does not terminate it
    ansible-playbook example.yml --ask-vault-pass  --skip-tags "self_destruct"

License
-------

BSD

Author Information
------------------

https://github.com/jbabe
