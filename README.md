# Ansible Elasticsearch

[![Ansible Role](https://img.shields.io/ansible/role/7197.svg)](https://galaxy.ansible.com/detail#/role/7197)

Ansible role which manage Elasticsearch.

## Requirements

- ansiblebit.launchpad-ppa-webupd8
- ansiblebit.oracle-java


## Variables

Here is the list of all variables and their default values:

```
elasticsearch_user: elasticsearch
elasticsearch_group: elasticsearch
elasticsearch_key_url: https://packages.elastic.co/GPG-KEY-elasticsearch
elasticsearch_apt_repo: "deb http://packages.elastic.co/elasticsearch/2.x/debian stable main"
elasticsearch_max_open_files: 65535
elasticsearch_cluster_name: elasticsearch
elasticsearch_home_dir: /usr/share/elasticsearch
elasticsearch_plugins: []
elasticsearch_remove_plugins: []

elasticsearch_ik_enabled: no
elasticsearch_ik_url: https://github.com/lepture/ansible-elasticsearch/releases/download/v0.1.0/elasticsearch-analysis-ik-1.7.0.zip
elasticsearch_ik_version: 1.7.0
```


## Usage

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
      - ansiblebit.launchpad-ppa-webupd8
      - ansiblebit.oracle-java
      - lepture.elasticsearch

License
-------

Licensed under the BSD License. Created by [Hsiaoming Yang](http://lepture.com/).
