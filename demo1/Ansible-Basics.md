Inventories \
Ansible Ad-hoc commands \
Ansible Playbooks \ 
Jinja2 for templating \
Create a playbook that installs, configures Nginx web server on both Ubuntu and Redhat and templates the deployment of a web app.

Inventories:\
Text file contains host details (because Ansible dont know what to do w/o host details) \
Static or Dynamic (static)\
Contains important varibles define how Ansible connects to the hosts.\
To check the ansible connection to the host.\
`ansible linux -m ping -o`

Ansible Ad-hoc commands:\
Setup command: Gather information about the system `ansible ubuntu -m setup`
File command: Sets attributes of files, symlinks, directories etc.. `ansible linux -m file -a "path=/tmp/test state=touch"`\
Copy command: The copy module as per the output above uses checksums to validate whether the copy was needed and was successful `ansible redhat -m copy -a "src=hosts dest=/tmp/hosts"`

Ansible-Playbooks and Handlers:\
Playbooks are sequence of tasks can be executed in an order. (Sync or Async)\
YAML file
Orchestrate the steps\
Handlers - runs exactly once and notify the tasks
`ansible-playbook simple_playbook.yml` 

Jinja2 Templating:
 Ansible makes use of the Jinja2 templating language\
 `ansible-playbook jinja2_playbook.yml`
 
  

