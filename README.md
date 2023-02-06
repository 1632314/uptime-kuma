# Ansible role for deploying Uptime-Kuma in a docker container

This role deploys an uptime-kuma docker container using ansible.

## Requirements
This role requires that docker it's already installed on the target machine. For that you can use @geerlingguy rol for [docker](https://github.com/geerlingguy/ansible-role-docker).

## Role Variables
```yml
# restart policy for container
uptime_kuma_restart_policy: unless-stopped
# host port
uptime_kuma_port: 3001
# volume path
uptime_kuma_volume_path: /app/data
# container name
uptime_kuma_container_name: uptime-kuma
# user who will be the owner of the volume
uptime_kuma_user: kuma
```