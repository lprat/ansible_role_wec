# ansible_role_wec
Ansible role Wec based on palantir (https://github.com/palantir/windows-event-forwarding)

## Playbook sample
```
#!/usr/bin/env ansible-playbook
---
- name: Install wef server
  hosts: all

  roles:
    - role: wef
```
