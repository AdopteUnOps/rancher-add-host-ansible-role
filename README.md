# docker-ansible-role

Ansible role to register host into rancher environment.

Requirements
--------------
Docker needs to be installed.

Mandatory Variables
-------------------
```
rancher_api_key: "mykey"
rancher_api_secret: "mysecret"
rancher_project_name: "default"
rancher_project_id: 1234
```
Role Variables
--------------

```
custom_host_tags: ""
rancher_agent_image: "rancher/agent:{{rancher_agent_version}}"
rancher_agent_version: "v1.2.6"
rancher_master_url: "http://localhost:8080"
rancher_agent_ip: "{{ ansible_default_ipv4.address }}"
```
License
-------

Apache License 2
