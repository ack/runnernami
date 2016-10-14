# Running with Bitnami

Bitnami Ansible Catalog

## Dev/Test

in a virtualenv: 

`pip install ansible==2.0.2.0 clc-ansible-module`

`export ANSIBLE_LIBRARY=$(python -c 'import clc_ansible_module; import os; print os.path.dirname(clc_ansible_module.__file__)')`

`export CLC_V2_API_USERNAME=<login>`

`export CLC_V2_API_PASSWD=<password>`

`ansible-playbook -vv -e @/tmp/vars.yml playbook.yml`

