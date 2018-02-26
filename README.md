# Prerequsites
### 1. Have local ssh key generated
[Generate ssh key](https://docs.typo3.org/typo3cms/ContributionWorkflowGuide/Appendix/OSX/SSHKeyOSX.html)
### 2. Acquire DigitalOcean API TOKEN
Login to digitalocean click API on top, generate API. Save TOKEN to environment.

In terminal type:
```shell
export DO_API_TOKEN="YOUR_API_TOKEN_HERE"
```
or append above command in your `~/.bashrc`

### 3. Install Ansible
Have *python2* and pip installed on your computer.
```shell
pip install ansible
```
note: it has to be python2
# Run provision.yml
```shell
ansible-playbook provision.yml
```
