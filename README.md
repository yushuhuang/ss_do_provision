# Prerequsites
## Have local generated ssh key
## Acquire DigitalOcean API TOKEN
Login to digitalocean click API on top, generate API. Save TOKEN to environment.

In terminal type:
```shell
export DO_API_TOKEN="YOUR_API_TOKEN_HERE"
```
or append above command in your `~/.bashrc`

## Install Ansible
Have python2 and pip installed on your computer.
```shell
pip install ansible
```
# Run provision.yml
```shell
ansible-playbook provision.yml -e "pass=user_pass ansible_sudo_pass=user_pass"
```
