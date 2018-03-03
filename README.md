# Prerequsites
### 1. Have local ssh key generated

```shell
ssh-keygen
```
### 2. Acquire DigitalOcean API TOKEN
Login to digitalocean click API on top, generate API. Save TOKEN to environment.

```shell
export DO_API_TOKEN="YOUR_API_TOKEN_HERE"
```
or append above command in your `~/.bashrc`

### 3. Install Ansible
Have *python2* and pip installed on your computer.
```shell
pip install ansible
pip install dopy
```
note: it has to be python2
# Run provision.yml
```shell
ansible-playbook provision.yml
```
