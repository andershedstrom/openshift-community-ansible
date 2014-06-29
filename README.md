# ANSIBLE

This cartridge provides Ansible so the machine can be used as a Ansible Control Machine

To get Ansible to work on Openshift, you need to use [this version of Ansible](https://github.com/andershedstrom/ansible), I've added a possibility to configure where to look for and write to the _known_hosts_ file using a environment variable, **ANSIBLE_SSH_KNOWN_HOSTS**. This is because cartridges may never write to _~/.ssh_, so Ansible won't play nice with you unless you can specify where to find the _known_hosts_ file.
