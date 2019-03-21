# aerospike_upgrade_demo
Demo of the aerospike upgrade playbook, showcasing the aerospike_migrations module

Read more about the module here:
https://docs.ansible.com/ansible/devel/modules/aerospike_migrations_module.html

The module code lives in the ansible core repo here:
https://github.com/ansible/ansible/blob/devel/lib/ansible/modules/database/aerospike/aerospike_migrations.py

Setup:
  1) `mkdir -p ~/.ansible/plugins/modules/database/aerospike`
  2) `cp aerospike_migrations.py ~/.ansible/plugins/modules/database/aerospike`
  3) Install ansible if you don't have it already. I'm using ansible v2.7.5 with Python 3.7.1, but I believe it will work with earlier versions too. The reboot module will not be present in <2.7 versions of Ansible I believe.
  
Running it:
  1) `ansible-playbook -i myinventory aerospike_upgrade_demo.yml`
  2) Have a snack, or pretend you're working maybe?
