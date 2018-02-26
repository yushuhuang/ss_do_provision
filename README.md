# Prerequsiite
## Acquire DigitalOcean API TOKEN
Login to digitalocean click API on top, generate API. Save TOKEN to environment.

In terminal type:
```shell
export DO_API_TOKEN="YOUR_API_TOKEN_HERE"
```
or append above command in your `~/.bashrc`

## Install Ansible
Have python2 and pip install on your host computer.
```shell
pip install ansible
```

## Generate hased password for vm
Linux
```shell
mkpassed --method=sha-512
```
mac
```shell
pip install passlib
python -c "from passlib.hash import sha512_crypt; import getpass; print sha512_crypt.using(rounds=5000).hash(getpass.getpass())"
```

# Run provision.yml
```shell
ansible-playbook provision.yml -e "user_name=your_user_name hashed_pass=your_hashed_pass ansible_sudo_pass=your_vm_passwd"
```