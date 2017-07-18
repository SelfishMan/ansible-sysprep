# Ansible role: sysprep
This role is based on [virt-sysprep from libguestfs](https://github.com/libguestfs/libguestfs/tree/master/sysprep) with most tasks implemented.  Notable exceptions are that this role does not:
* Change UUID of LVM volume groups
* Change UUID of any disks
* Remove extra users

## Usage
Include the config below in your playbook
```yaml
- roles:
  - { role: sysprep, become: true }
```

