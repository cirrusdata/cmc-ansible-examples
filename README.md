# Cirrus Migrate Cloud Ansible Playbook Examples

This repository is a series of Ansible Playbooks that automates live migrations end-to-end, from installation to migration and cutover, using Cirrus Data Cloud's REST API.

Visit https://cloud.cirrusdata.com to get started today.

***⚠️ THESE PLAYBOOKS ARE PROVIDED AS EXAMPLES. IT IS NOT DESIGNED AS AN REUSABLE MODULE AND WILL NOT WORK AS-IS ON ANY ARBITRARY ENVIRONMENTS WITHOUT CUSTOMIZATION AND MODIFICATIONS.***

# Prerequisites
Before you start, you should have:
- Sufficient knowledge on Ansible, including how to execute Ansible Playbooks, specify variables, etc.
- Hands-on experiences with Cirrus Migrate Cloud via Cirrus Data Cloud and sufficient understanding on concepts including installation, block migration, cutover process., etc.

Contact Cirrus Data's Professional Service for more information.


# Playbook Design
These playbooks are designed to run as standalone playbooks. No additional user actions are needed other than executing the playbooks.

## Inventory
Ansible Inventory should contain hosts to be included in the operations.  

## Variables / Credentials
Each playbook example comes with a **vars.example.yaml** file. When executing playbook, a **vars.yaml** file should be created with the same variables for execution.

# Playbooks

## Azure Windows Migration from Premium SSD v1 to v2

Install CMC, Resize Filesystems, Auto Allocate Storage Volumes using integration, create migration session
```
ansible-playbook playbook/migrate-to-v2.yaml
```

Cutover Process
```
ansible-playbook playbook/cutover-to-v2.yaml
```


## Licensing
This project is licensed under the Apache License, Version 2.0. See
[LICENSE](https://github.com/docker/docker/blob/master/LICENSE) for the full
license text.

## Support
This project is published as-is and no community support will be provided. [Contact](mailto:info@cdsi.us.com) Cirrus Data Professional Service Team to learn more. 