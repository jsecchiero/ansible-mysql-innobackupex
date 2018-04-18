# ansible-mysql-innobackupex

backup mysql using innobackupex

## Role Variables

### `innobackupex_source_server`
- Default value: **no**

### `innobackupex_destination`
- Default value: **no**

### `innobackupex_parallel`
- Default value: **3**

### `innobackupex_destination`
- Default value: **3**

## Example
```
- name: copy master mysql data
  hosts: 127.0.0.1
  roles:
    - role: jsecchiero.ansible-mysql-innobackupex
      innobackupex_source_server: 1.1.1.1
      innobackupex_destination: /mnt/backup
```
