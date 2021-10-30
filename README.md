# README

# far from being perfect

Ansible Playbook, to Setup K8-Cluster on Debian 11 minimal installation (only SSH).

This Playbook does not cover Security.

### Export ANSIBLE_VAULT_PASSWORD_FILE for Vaultpass
```bash
export ANSIBLE_VAULT_PASSWORD_FILE=./.vault_pass
```

### Install Requirements
You can also include it in a requirements.yml file and install it via ansible-galaxy using the format:
```
ansible-galaxy collection install -r requirements.yml
```


### run playbook
```
ansible-playbook debian-k8-cluster.yml -i hosts
```

### If not working Try
```
ansible-playbook debian-k8-cluster.yml -i hosts -u root -e "@vaultvars.yml"
```

