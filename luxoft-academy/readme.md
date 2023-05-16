First RUN
```
ansible-playbook inital_config.pb.yml -i inventories/aws_l/hosts.ini --ask-pass
```
or
```
ansible-playbook inital_config.pb.yml -i inventories/aws_l/hosts.ini --ask-pass -t ssh_key
```
to run only ssh key instalation.

To skip ssh key instalation use --skip-tags ssh_key
```
ansible-playbook inital_config.pb.yml -i inventories/aws_l/hosts.ini --skip-tags ssh_key -v
```