## Ansible Collection - alex.ansible_file

This is educational project for creating files

### Installation

```console
ansible-galaxy collection install git+https://github.com/Alex-Elfman/my_own_collection.git,ansible_file 
```

### Usage

`alex.ansible_file.ansible_file` module

```yaml
---
- name: create file
  hosts: localhost
  tasks:
    - name: create file
      alex.ansible_file.ansible_file:
        path: /tmp/test
        content: |
          333
          444
          555
          666
```
`alex.ansible_file.ansible_file` role

```yaml
- hosts: localhost
  roles:
    - alex.ansible_file.ansible_file
```
