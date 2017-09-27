# docker-ansible-role

Ansible role to register host into rancher environment.

This role assume that you have an apikey file in {{ inventory_dir }}/group_vars/{{ rancher_project_name }}/apikey.yml containing the following variables :
* rancher_api_key_project_token
* rancher_api_key_project_secret
* rancher_project_id

Requirements
--------------
Docker needs to be installed.

Role Variables
--------------

```
custom_host_tags: ""
rancher_agent_image: "rancher/agent:{{rancher_agent_version}}"
rancher_agent_version: "v1.2.6"
rancher_master_url: "http://localhost:8080"
rancher_project_name: "default"
```
License
-------

Apache License 2
