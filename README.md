# Ansible role `java`

An ansible role for installing Java.

Tested under:
* Amazon Linux 2017.03
* CentOS 7.4
* Fedora 25
* Ubuntu 16.04

## Requirements

No requirements

## Role Variables

| Variable       | Default | Comments                              |
|:---------------|:--------|:--------------------------------------|
| `java_version` | 8       | Java version                          |
| `java_devel`   | false   | false: Install JRE, true: Install JDK |

## Dependencies

No dependencies

## Example Playbook

```yaml
---
- name: example
  hosts: all
  become: true
  vars:
    java_version: 8
  roles:
  - lechuckroh.java
```

## License
MIT
