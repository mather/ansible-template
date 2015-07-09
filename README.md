Ansible project template with Vagrant
=====================================

Based on [Ansible playbook best practice](http://docs.ansible.com/playbooks_best_practices.html)

### Directory Structure

```
.
├── bin/
│   └── create_role
├── production      # inventory file for production servers
├── staging         # inventory file for staging environment
├── group_vars/
├── host_vars/
├── filter_plugins/ # if any custom filter plugins, put them here (optional)
├── library/        # if any custom modules, put them here (optional)
├── roles/
│   └── common/
│       ├── defaults/
│       │   └── main.yml
│       ├── files/
│       ├── handlers/
│       │   └── main.yml
│       ├── meta/
│       │   └── main.yml
│       ├── tasks/
│       │   └── main.yml
│       ├── templates/
│       └── vars/
│           └── main.yml
├── Vagrantfile          # Vagrant settings
├── vagrant_hosts        # inventory file for vagrant provisioning
└── vagrant_playbook.yml # playbook for vagrant provisioning
```



### Scripts for ansible development

```
$ bin/create_role <role>
```

Create role directories under `roles` directory.