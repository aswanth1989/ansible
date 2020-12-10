Tags:\
Works well large playbooks\
Segmentation\
Skip the tasks \
execute only certain tasks.

`ansible-playbook nginx_playbook.yml --tags "nginx-template"`

Roles:\
Roles allow you to structure and group your playbook tasks and associated components. \
Larger projects are made easier to manage, roles are grouped with logical structure making them easier to share, roles can be written to target specific requirements

`ansible-galaxy init nginx`
`ansible-galaxy install elastic.elasticsearch,7.10.0 --force`

***Refactor the nginx playbooks to roles now***

