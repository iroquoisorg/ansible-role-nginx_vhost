# nginx_vhost

[![Build Status](https://travis-ci.com/iroquoisorg/ansible-role-nginx_vhost.svg?branch=master)](https://travis-ci.com/iroquoisorg/ansible-role-memcached)

Ansible role for nginx_vhost

This role was prepared and tested for Ubuntu 16.04.

# Installation

`$ ansible-galaxy install iroquoisorg.nginx_vhost`

# Default settings

```

nginx_vhost_host: ""
nginx_vhost_web_root: ""
nginx_vhost_web_port: 80
nginx_vhost_ssl_crt_path: ""
nginx_vhost_ssl_key_path: ""
nginx_vhost_ssl_crt_chain_path: ""
nginx_vhost_env_vars: []
nginx_vhost_basic_auth_location: "/"
nginx_vhost_basic_auth_users: []
nginx_vhost_force_ssl: false
nginx_vhost_force_ssl_location: "/"
nginx_vhost_nginx_user: "{{ nginx_user | default(\"www-data\") }}"
nginx_vhost_nginx_group: "{{ nginx_group | default(\"www-data\") }}"
nginx_vhost_server_aliases: []
nginx_vhost_php_version: "{{ php_version | default('7.1') }}"
nginx_vhost_fpm_socket: "/var/run/php/php{{ nginx_vhost_php_version }}-fpm.sock"
nginx_max_upload_size: "10M"
nginx_header_buffers: "8 32k"
nginx_log_type: ""
nginx_vhost_php: false

```

# Development

Please check [development guide](DEVELOPMENT.md) for details about developing and testing this role.
